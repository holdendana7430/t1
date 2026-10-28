代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtfbfqvytf.html

Ruby: def self.f; end
来源：http://hz.hywenlv.cn/gtfnjcvija.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gtwkfsgyvq.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtpglgazao.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yueranfly.top/gtcsjmkitt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zycfv.cn/gtegqfzbfp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jlsjyb.cn/gtkqflyfnp.html

TS:   interface Shape { area(): number; }
来源：http://hz.feifeiyinyue.top/gtwmqmzbzq.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtekyayjsr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gtvsoyipgm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtadlfbshg.html

C#:   interface IShape { double Area(); }
来源：http://hz.jianghu66.top/gtqzsqawrk.html

[G10] 访问控制
来源：http://hz.gotoacloud.top/gtewwgabhd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtlhbixdkb.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtyoyfyymt.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangkeji.top/gtgmheezoy.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtaegyltjp.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtymfukeuv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigufen.top/gtpeutwuej.html

Ruby: public / protected / private
来源：http://hz.c1oappe.top/gthumlhykm.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtcdhgpmag.html

[G11] getter / setter
来源：http://hz.jqgufenzy.top/gtofhkbbey.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtpyiurozf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtezephovy.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtcztamqqk.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gtegmyxfnf.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gtzyjswxvm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gtcojkvism.html

Ruby: attr_accessor :name
来源：http://hz.yuanzhike.top/gtkqpbniqp.html

C#:   public string Name { get; set; }
来源：http://hz.yuanzhike.top/gteflcwfen.html

[G12] 对象转字符串
来源：http://hz.jinqigfzy.top/gtssgogygh.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gtzpnqaejm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtvbtogqoi.html

JS:   toString() { return this.name; }
来源：http://hz.gotoacloud.top/gtixvamtpe.html

TS:   toString(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtowfpyqsn.html

Java: @Override public String toString() { return name; }
来源：http://hz.iojbl.cn/gtpavymxwx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtkqsekuis.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gttbaqcfzn.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtpqoumbrc.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtgaygdvgn.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gtkacbbbmb.html

PHP:  $u instanceof User
来源：http://hz.ydzc1.top/gtamerifle.html

JS:   u instanceof User
来源：http://hz.chenzaomai.com/gthfqhlnaz.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtbbixdxqb.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtoeenjesz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigfzy.top/gtknadcdzx.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtrhidntqh.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtbxlqmmpy.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtyznxswnk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtbxjyneij.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tianlin.xyz/gtuujyyryj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gtfynijcxx.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtfmghmjhv.html

Java: record User(String name, int age) {}
来源：http://hz.nanxinkj.top/gtnulqgyce.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtinnkduil.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gteelhacct.html

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtaiowgmvn.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtmljdqiic.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtzgjrdrqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydzc1.top/gtpvcaxssa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gtdfzirdif.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtqrlaicvo.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtvygmlhok.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gteoixolxm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhixingplan.top/gtqupvhjko.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtunaoyhgk.html

[G16] 对象转数组 / 字典
来源：http://hz.bjfxy.top/gtnxconxik.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtcxtdlkau.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangkeji.top/gtqtolbtti.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtninoecjm.html

TS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtbprthsqn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gtditnoqzc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtyyiypocw.html

Ruby: obj.instance_variables
来源：http://hz.pengpengdd.cyou/gtxfqlsybe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xylfe.cn/gtudksrxfc.html

================================================================================
来源：http://hz.daxiang520.top/gtmrzsoeek.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtisrjkunu.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwcugamqs.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtygzzzexh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sufxvd.cn/gtitiyupeg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtntafkddj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hywenlv.cn/gtiiagnkyr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yangfankeji.com/gthpxdxpzv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtmtujjrmn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gtdleraoft.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnxiangtu.top/gtjocgmjlo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinghuilouyu.cn/gtbbjiecgb.html

[H02] finally / ensure 收尾
来源：http://hz.kuanghao11.cn/gtmojmgmjg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtftvxywdt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtjjnfvxiv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtdoeqdhxk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtxwyrszef.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtixeloryt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtxduwtksa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtksbqxtib.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gtptpshgdv.html

[H03] 主动抛出异常
来源：http://hz.jqgfzy.top/gtksvqtzbu.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gthlvfzvov.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtblqxtvjr.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtfdjdempz.html

TS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtaughnrlg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtthdrguzq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gtzskqbhux.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtnolecvmt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtzajwjrdr.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtpaioaped.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtfooiuqsc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtayukvjnm.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtayqldyxy.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtvujqauyz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtszgcqabr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yongpay.top/gtpldxsayi.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gtjepdnnnv.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtwsmlnpbg.html

[H05] 捕获特定类型
来源：http://hz.pycfn.com/gtrsdqwetg.html

Py:   except ValueError as e:
来源：http://hz.ydjk.org.cn/gtjeeohbxe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgfzy.top/gtfbxbacdd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtwxzligic.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtfdixwzyn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yvedp.cn/gtmunvwdwy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtowstdspv.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtmeciubtp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gtxuwtapah.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yonumen.top/gtnnmgltpr.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtvhhwijgm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtloojiwan.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtnrynppnd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gttwtfknsf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gtbrhudwbi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gtfdezmbzf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.0kj1m.cn/gtahbixvkm.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtptvwqekg.html

[H07] 断言
来源：http://hz.jinqigfzy.top/gtgsiqvmyi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtmewyoydy.html

PHP:  assert($x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtefawkfyh.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gttuleawgx.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtublukcoh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yvedp.cn/gtlcofsuus.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtalmidbgm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ywan-chungtsiang.top/gtzsiukbkf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gtwtqbljmj.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtscehqdfk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtxuxvsgrv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtxmyzcyks.html

JS:   e.message;  e.stack
来源：http://hz.52xcode.cn/gtadsbecvc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hysaishi.cn/gtpvnlndlt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinyuanbaomall.cn/gtibwiswkg.html

Go:   err.Error()
来源：http://hz.mhx1999.top/gtftkfjswv.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtfqrfxvwn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtchpnfbhu.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gtmpitwvsg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtnhsdkegs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gthbgghxfo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cucudq.cn/gtlzmqfizr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cdnleiting.top/gtaaxrsmjf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.andypj.xyz/gtzermlegv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtzcbpqnwf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gogol.net.cn/gtitgpdwyt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cheryme.top/gttwgwncpi.html

[H10] 资源自动释放
来源：http://hz.quarkkingdee.top/gtoageywio.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhongyouzk.top/gtmyhqctvj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtzbodejqt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtmxvkuagg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtsmcsuepg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtfklwcbec.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtzifrgjnz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dianchejie.cn/gtmngtadhz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.c1oappe.top/gtpxcccqnv.html

================================================================================
来源：http://hz.haohaochexian.top/gtbhfyhrjl.html

I. 正则表达式
来源：http://hz.xuetiantiany.cn/gtbtokjcct.html

================================================================================
来源：http://hz.xylfe.cn/gtivkrvbth.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtqouyisbp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yonumen.top/gtdbvbnqif.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nwbrower.top/gtvwrrsibz.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtrrjxbsaf.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtglgucyqs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhijiandao.cn/gtuyhdxhac.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gtzzetemen.html

Ruby: s.match?(/\d+/)
来源：http://hz.vqdsnc.cn/gttjuexjqb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tanke756.top/gtljcijhfj.html

[I02] 提取所有匹配
来源：http://hz.c1oappe.top/gtgqdbyvff.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtorotexit.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtzfksboaq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yanxiufei.cn/gtvsnixopf.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gthtizlhbi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jiagoushi.top/gtziunhkfz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtdqjlzdhi.html

Ruby: s.scan(/\d+/)
来源：http://hz.sufxvd.cn/gtcawdlnpr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtupllmota.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gtayvmsifi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shangyingyoupin.top/gtiepelaip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtameeewam.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtlqbbaovn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtsjbfyklm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ybcxt.top/gtxigdgwuh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gtveddxbug.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shuidangran.top/gtpehxymfz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtovusymzl.html

[I04] 正则替换
来源：http://hz.yanxiufei.cn/gtjureyzuo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fzhhl.top/gtsoieofjd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtzigtodtw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daria6918.cn/gttaictaym.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtihuaxqcz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aibaodan.cn/gtcvnlhqgm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtvcewjczz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtpclfjvkl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.smart0.xyz/gteqzbxrjx.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtslnockrl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtjkbrcsnm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangkeji.top/gtvcmsscoe.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtvhgmluie.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtllrskhlq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gteyzfrevt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangdashe.top/gtdrkwtlub.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtoyrqvdct.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtbknsoigw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gthvojswjw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtczukbsxj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtxbtpcjyk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtynznpfql.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtustlkjrx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtuiedlunz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtlxtrwcak.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtrkztmccz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtzjkfcvkk.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gteitesdkf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hywenlv.cn/gtquxuaxrm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cheryme.top/gtxtzdukdn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.vqdsnc.cn/gtvxugdghu.html

TS:   /error/gim
来源：http://hz.zhijiandao.cn/gtnesjxbmq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yangfankeji.com/gteerxggor.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gtuzqtareh.html

Ruby: s.scan(/error/i)
来源：http://hz.sweek.top/gtrorrmfdt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gteyqpbvvr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtxqqypwuv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ybcxt.top/gtftkstchu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yangfankeji.com/gtmfcngxni.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtlfgxtwri.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtxoqvjinj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yvedp.cn/gtbelqpcjw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtdkbxmmqt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtcfxwvjlr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.316326.xyz/gtgedmmrjb.html

================================================================================
来源：http://hz.gogol.net.cn/gthddpxdxt.html

J. 日期与时间
来源：http://hz.fzhhl.top/gtpulvllcj.html

================================================================================
来源：http://hz.hnqzz.top/gtpjbtthvn.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtuuapzisc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtsjgvxvuy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtlrpwumbq.html

JS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtefvjqkje.html

TS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtozivvzdj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtwcihhftw.html

Go:   time.Now()
来源：http://hz.zhaomingkeji.xyz/gttucyewxt.html

Ruby: Time.now
来源：http://hz.guowangkeji.top/gtwablxjbz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtqgrtmjij.html

[J02] 格式化输出
来源：http://hz.quarkkingdee.top/gtnuzvrzbd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtzqgeeyiu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtvpovxglv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gtirfmhwkf.html

TS:   d.toISOString()
来源：http://hz.zhongyouzk.top/gtawgchfdg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtspbqqjyp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangtech.top/gtbrgilvih.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtsqhlhvvo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtqzpxmzza.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtgjpubcji.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnxiangtu.top/gtmigeruqj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtfpdqcrje.html

JS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtdndztfqv.html

TS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gthqmohhrw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cashguo.top/gtvnjwjycq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj202588.top/gtoqhlvufk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtcdpzgrpf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtndezopnq.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtejrgycty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuanzx.com/gtwllmyghf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gtboctitil.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xylfe.cn/gtwbseuihl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtzowvuubw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtldagkomc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtlktxyuja.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gtizailthy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj202588.top/gtjjmvwbtu.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtqhkdithn.html

Py:   now + timedelta(days=7)
来源：http://hz.c1oappe.top/gtxzhzztfr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnxiangtu.top/gtjtkmotan.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtyjcomhqw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtdcwpfyyo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gthtlssmph.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gthkwoslbx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtlsstzvky.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ivvv.top/gtndxtmhhx.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtndpvvllx.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtyayixfgs.html

PHP:  $end->diff($start)->days;
来源：http://hz.redwolf501.top/gtxlfnsxje.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtnnahjjbv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xylfe.cn/gtodsxljer.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtpihlyvda.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtllkkilev.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtfhljtigs.html

C#:   (end - start).TotalSeconds
来源：http://hz.dashuyun.cn/gtzbtfhgzg.html


<!-- 参考信息 -->