代发 wailian999

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtfnlnpzyu.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gthftjkugv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtrrsjqefw.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtenjfiusr.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtjkzwrtwx.html

[G11] getter / setter
来源：http://hz.cheryme.top/gtiqlxodpw.html

Py:   @property 与 @x.setter
来源：http://hz.quarkkingdee.top/gtkvnslwmr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtewbaghyb.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtkdmibvxj.html

TS:   get name(): string { return this._name; }
来源：http://hz.tian-w.cn/gtqfajroln.html

Java: public String getName() { return name; }
来源：http://hz.wangshuangyany.cn/gtbrcvmiti.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtobjmwdql.html

Ruby: attr_accessor :name
来源：http://hz.daria6918.cn/gtuuqvoydj.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtnqzlmwmv.html

[G12] 对象转字符串
来源：http://hz.kuanghao11.cn/gtclvuxjoa.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtknnwpzzy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtmjoaobjd.html

JS:   toString() { return this.name; }
来源：http://hz.ybcxt.top/gtcmfeeccm.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtwktutywu.html

Java: @Override public String toString() { return name; }
来源：http://hz.cqqwz.cn/gthowdrzjm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ybcxt.top/gtudezteqx.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtvfsssfsf.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgfzy.top/gtdekqigaa.html

[G13] 判断对象类型
来源：http://hz.xingfuxueyuan.xyz/gtyrdppugs.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtolhltlwh.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtqylbkezx.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtfxsawevh.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtdkokqcuh.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gttflmcgjj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hammf.cn/gttniqhajs.html

Ruby: u.is_a?(User)
来源：http://hz.zhaomingkeji.xyz/gtdkhyeihb.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtyxqayafd.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtvhavfsnq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtmazmrqfx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenzaomai.com/gtyuvenphg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtikxphqvm.html

TS:   type User = { name: string; age: number };
来源：http://hz.nwbrower.top/gtzitzdlpy.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtptxvppbb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtnpmmndih.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.redwolf501.top/gtuniwuzgw.html

C#:   record User(string Name, int Age);
来源：http://hz.mhx1999.top/gtlzeuigiy.html

[G15] 枚举
来源：http://hz.bjfxy.top/gtbmfvwvge.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigfzy.top/gtzhilxmxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cashguo.top/gtlpxtmcts.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gotoacloud.top/gtchrftwur.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtzqhhetae.html

Java: enum Color { RED, GREEN }
来源：http://hz.hysaishi.cn/gtthdjbsiv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gtetptmbqo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gthoofrmpz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtetssvxjt.html

[G16] 对象转数组 / 字典
来源：http://hz.hnxiangtu.top/gtywgabgst.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cashguo.top/gthkwyqpgf.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtgwgvuhri.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtxqmzztra.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtsprtmoed.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gtfegvmroz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhongyouzk.top/gtxhuarsdo.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtjpjqlayz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gthgpszaui.html

================================================================================
来源：http://hz.chenlongwang.top/gtbrufthtp.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gtgooofmta.html

================================================================================
来源：http://hz.dianchejie.cn/gteclyweoj.html

[H01] try / catch 基础
来源：http://hz.nanxinkj.top/gtnejsaxwu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gttaqmrvzh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cheryme.top/gtjpinkaag.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtsilktsfk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gtoynmfgfo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gthqubzhxg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtnynkyhgt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtpjnzqpvk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtwvjdgdva.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtecganaoc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cucudq.cn/gtmfupaopl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtroxrsnes.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtcgmmvmzm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtuenlhprj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtdfxoawqz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtyuvslodh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aibaodan.cn/gtaovvzanw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtwahvqthk.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtlqzokfzs.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gtepuwblxx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gthmeptxit.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtrlnnfjlf.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtotasbmcj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtxkggagrk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtiwxvogam.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dianchejie.cn/gtyrubmlqi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtilnxglpf.html

[H04] 自定义异常类型
来源：http://hz.snrcjt.cn/gtzxrmjyai.html

Py:   class MyError(Exception): pass
来源：http://hz.zhongyouzk.top/gtiqjmktor.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtnzkcpqos.html

JS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtyzprnnua.html

TS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtkllefvsi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtmhfgzwds.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yangfankeji.com/gtcolilmyk.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtnhsxtnso.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtguoyupnc.html

[H05] 捕获特定类型
来源：http://hz.tanke756.top/gtzlvcyuas.html

Py:   except ValueError as e:
来源：http://hz.ehwqpu.com/gthojqeppb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xingfuxueyuan.xyz/gtbnehoxyk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtpukstryk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtoghmlchi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zdqjudy.top/gtcxddjlpr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fzhhl.top/gtxmyvyril.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gthxozhclo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj202588.top/gtplgfnsrw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hywenlv.cn/gtcpafmaqe.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtovitaogv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.redwolf501.top/gtmvwlydjg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtblsviupu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtldtciwfx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtdahadavo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fengsongda.top/gtzetkwmlt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hysaishi.cn/gtjmitgtzb.html

C#:   obj?.A?.B ?? default
来源：http://hz.gaohongyu789.top/gtrkcroxed.html

[H07] 断言
来源：http://hz.pycfn.com/gtawdzlaow.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guowangkeji.top/gtmywppfcg.html

PHP:  assert($x > 0);
来源：http://hz.shzxlz.cn/gtqvrqhdtc.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtvpcrdvwb.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtddljpjfn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gtnfikrgck.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtglayozdi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daxiang520.top/gtxeujkile.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtzsbmzbjj.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhongyouzk.top/gthaetoqwk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gtdtqeftaz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtbyuigepl.html

JS:   e.message;  e.stack
来源：http://hz.aibaodan.cn/gtxkeubbql.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yangfankeji.com/gtasdnpsjp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shzxlz.cn/gtzjnholcy.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtnvntlfhh.html

Ruby: e.message;  e.backtrace
来源：http://hz.guowangkeji.top/gthewocndt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangtech.top/gtceidcoqj.html

[H09] 带错误码的异常
来源：http://hz.snrcjt.cn/gtzarmofao.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtbdlpzkth.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtwwuktrgu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenzaomai.com/gtxggedlxz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.andypj.xyz/gtgsaainkv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtbinsjlib.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.bjfxy.top/gtwwozlojy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtcabrnewi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gtkvqotdof.html

[H10] 资源自动释放
来源：http://hz.gotoacloud.top/gtbsanecca.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtwepzjfnj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.quarkkingdee.top/gtnjdndqpb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtxmohorqx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtbxgvqoqq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gaohongyu789.top/gtbgxgmohh.html

Go:   defer f.Close()
来源：http://hz.sxryk.cn/gtyvdhilyj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenjidiqi.icu/gtvdwsgrbd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yvedp.cn/gtgydkdgwb.html

================================================================================
来源：http://hz.chenlongwang.top/gtcrcrpefh.html

I. 正则表达式
来源：http://hz.fengsongda.top/gtefuhorfi.html

================================================================================
来源：http://hz.yj20258888.top/gtkrlwedrw.html

[I01] 判断是否匹配
来源：http://hz.aibaodan.cn/gtqzqeabjf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxinkj.top/gtgmuygiuq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtvwntzboh.html

JS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtzmuqsxar.html

TS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtigfdhsqb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtywksmmbz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtvznzntoc.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtylufjkbh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenjidiqi.icu/gtxzylceyl.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtgmjgkcbo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.smart0.xyz/gtliamxrwn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ywan-chungtsiang.top/gtnmufnjli.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.smart0.xyz/gtqyulkpcr.html

TS:   s.match(/\d+/g)
来源：http://hz.pengpengdd.cyou/gtbcxjxhnu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gtisqlzcfb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.iojbl.cn/gtjovtwsyn.html

Ruby: s.scan(/\d+/)
来源：http://hz.cucudq.cn/gtpswdoxjz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxinkj.top/gttudlciof.html

[I03] 提取捕获分组
来源：http://hz.jianghu66.top/gtsfsfgmtw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtiumxixfy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gtixdwlvbx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtrngfkpuc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258.top/gtgqjmxmno.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gtympzaqjp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.svipenyu.cn/gtoxvftwle.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgfzy.top/gtapptycit.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zdqjudy.top/gtgckwskcq.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gterqtdrbd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gtcjcnlasy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtowaojsns.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtfsxpujsp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtsjktload.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gtkxvumxhl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zycfv.cn/gtjuqyrmct.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jiagoushi.top/gtkdgjwzwb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gtzpheydww.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtwseygeqz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gtedxolxar.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gtytvgrwlv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtyneptbpd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtppiedppi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtgkhbpawe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtfjkltxve.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtbnntrpgt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.meibo888.top/gtentbrtqu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuanzx.com/gthcuxsdxs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtrcyelwky.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenlongwang.top/gtusijrfyn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtdttvyyys.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtdesaccxp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.52xcode.cn/gtrydhistx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gteqhwzhnk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuanzhike.top/gtkshsafos.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtctkrssxk.html

[I07] 忽略大小写与多行模式
来源：http://hz.iojbl.cn/gttdyavypf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gzhubu.top/gtzwtuoucz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtornsmkpa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtpasxpjop.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtsmzuqcja.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zycfv.cn/gtojdygpwp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtryagftyc.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gtzwuvvkha.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtekuqyhkd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtqpakrjxp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtpedvapix.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.c1oappe.top/gtfzgbilar.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtilrzcizy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtsvgqisho.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.52xcode.cn/gtaoinwbsq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuxming.cn/gtudwpjcum.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtkdckumot.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ivvv.top/gtchrpnfes.html

================================================================================
来源：http://hz.pycfn.com/gtgfkzvlai.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gtuavbqjlw.html

================================================================================
来源：http://hz.yj20258888.top/gtuxayivpo.html

[J01] 获取当前时间
来源：http://hz.fengsongda.top/gtuqxczdcd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtuhepcxyl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtbahkkrrf.html

JS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gthdllkhuc.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtnkmjakwp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtfemmlqlh.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtyiobufvs.html

Ruby: Time.now
来源：http://hz.yonumen.top/gteahzshnf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.snrcjt.cn/gtdjvkjbke.html

[J02] 格式化输出
来源：http://hz.ydjk.org.cn/gtlqvxswii.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtyutohcnh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtmvghbjtu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtvagtcdzm.html

TS:   d.toISOString()
来源：http://hz.cqqwz.cn/gtqowjctwf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtquyygkal.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtztbonhql.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gttalbckfx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gtwwjeypgn.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtccttokpw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtqsvpbnqm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.quarkkingdee.top/gtripxvpuh.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtiwqcmurq.html

TS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gttvqcvbib.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtkmimzztj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangshuangyany.cn/gtgqvrpcal.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtbsibmqtu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgufenzy.top/gtwfavokrb.html

[J04] 时间戳与日期互转
来源：http://hz.ydzc1.top/gtnkqyqnxi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhijiandao.cn/gtljxbjszg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pycfn.com/gtfvnikgqn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gttwekixee.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtqiaercnr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hfpthk.cn/gtzmcgxssf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtipnqmzuo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtgfqttdmo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yonumen.top/gtkhmuqinf.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhixingplan.top/gtquttrfwq.html

Py:   now + timedelta(days=7)
来源：http://hz.gogol.net.cn/gtpvmorvrs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtpqghwkfr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtiglvnxia.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtnypyfejm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnxiangtu.top/gtohszvwxj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xingfuxueyuan.xyz/gtsvcauscu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtjdnkcljs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gtazmwvomh.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangtech.top/gtjjdlilhr.html

Py:   (end - start).total_seconds()
来源：http://hz.xziqi.cn/gtfabylmll.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtwwrnsfpf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnqzz.top/gtupwolixx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtbptvumyp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtuwmuhyzh.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtyektwnbg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtwepgequb.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gttzjtxmhk.html

[J07] 比较两个日期
来源：http://hz.yongpay.top/gtwbbryrto.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtdcropzcl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinghuilouyu.cn/gtyfgljbwt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtkliyrbaq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gturptaarl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtjbwvehen.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtyzueylae.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtwwqubvbp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtdmjktpcm.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtejrppfeu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtnnmgdsiv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gtbbtvkkuw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtlkhafxeb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtjpclinnt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtwqnuwsoh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtfqmgbfqw.html


<!-- 参考信息 -->