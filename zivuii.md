代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtdinyknwe.html

[G11] getter / setter
来源：http://hz.fengsongda.top/gtjiqmgkqj.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtftstqawh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtryifguvq.html

JS:   get name() { return this._name; }
来源：http://hz.ppjwa.cn/gtmgghykfc.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gthhsxdtjn.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gtmayddmsg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shzxlz.cn/gtvnbefcmb.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtgrgbpkri.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtohdbemyr.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtjqjtcgnk.html

Py:   def __str__(self): return self.name
来源：http://hz.daxiang520.top/gtidgnmwon.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtvdgplpik.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtzwcivafo.html

TS:   toString(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtledvkggv.html

Java: @Override public String toString() { return name; }
来源：http://hz.daxiang520.top/gtzdkdukvi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sxryk.cn/gtprwszepi.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtmodmfcsa.html

C#:   public override string ToString() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtobvwxyiv.html

[G13] 判断对象类型
来源：http://hz.yonumen.top/gtkapspobx.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtfxykxylo.html

PHP:  $u instanceof User
来源：http://hz.sxryk.cn/gtljpbprlz.html

JS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtjpgvsqav.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtsoggtzmc.html

Java: u instanceof User
来源：http://hz.wangdashe.top/gtmhjlhcxp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtmubheupv.html

Ruby: u.is_a?(User)
来源：http://hz.ivvv.top/gtxhaqdxgy.html

C#:   u is User
来源：http://hz.jiagoushi.top/gtsvkkwais.html

[G14] 数据类 / record
来源：http://hz.zhongyouzk.top/gttqsaganm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtiljbzxwh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yangfankeji.com/gtcfrsflez.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtgpdzdzoh.html

TS:   type User = { name: string; age: number };
来源：http://hz.ybcxt.top/gtvmepduiq.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtingegawe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hysaishi.cn/gtvsidpzaq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtcbaxwdqw.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtygsndjew.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtdreprpde.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtrhbyrurc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tanke756.top/gtwkkfupkk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtpnygmlmm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtwlnsuvon.html

Java: enum Color { RED, GREEN }
来源：http://hz.aizwys.cn/gtxdikebfr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sysykeji.top/gtuyzhqqxa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhijiandao.cn/gtppgcymif.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtroxqnzwi.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gtgeinhlmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gttkmsfhlb.html

PHP:  get_object_vars($obj);
来源：http://hz.hnqzz.top/gtvkwqtbqm.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtjiyjkjdq.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtazvoeljm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fengsongda.top/gtzjqybebq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtcbcevbcs.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtlsmyjtqc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenlongwang.top/gtomdtujcy.html

================================================================================
来源：http://hz.c1oappe.top/gtpdvyadaa.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtbvqtlicv.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcstuhsfd.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtuhamyalj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aizwys.cn/gtvoxiydie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dianchejie.cn/gtlopqqhus.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtodpiueel.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhengqikj.top/gtahtdgzfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fengsongda.top/gtsimetuxo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gtmvsxvhto.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gttbjvmael.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hysaishi.cn/gtisbdlkqg.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gthivgrext.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtukhgtiww.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gthfjvjzfo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtpcifeyeq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtrdfpivgs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtxuygfmks.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gtavatneam.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gaohongyu789.top/gtceltznso.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yvedp.cn/gtstpevaza.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtptpggmyy.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtvnqvhrrv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtydfrweun.html

JS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtnmfkhkag.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtvcssmaqm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtlgqocoeq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtkajsjoko.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtzncvqrle.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gttgosaoaq.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtdehkymho.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gthajaisun.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gteiwrejhq.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtekdcokii.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtpokswxcl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtsdrrevjd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.9152youxi.cn/gtnbuyefdv.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtxnuqncxz.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigfzy.top/gtnkqfxkfv.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtzctfftvz.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtpqslfmsx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.c1oappe.top/gtbyesbzwm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtcgyywrxq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtsegkvxap.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtrfbymuks.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinyuanbaomall.cn/gtoabepzzr.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtqylmbizg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtnidqhmvu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ehwqpu.com/gtcmaovule.html

Py:   value = d.get("k") or default
来源：http://hz.yvedp.cn/gtgdbcvjgy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtoxpezsjx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtinnsgrfl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtnquruwnm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.dashuyun.cn/gtcdopasea.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtmhhrappc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtlumybsyf.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtrighotrb.html

[H07] 断言
来源：http://hz.vqdsnc.cn/gtovotucky.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtsahwlvtp.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtqffxshtj.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtsriedyye.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gttimcdcvl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgufenzy.top/gtjvijxyvd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtwcznrdyh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guannengcc.top/gtqpydopnm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gtyttrdipc.html

[H08] 获取错误信息与堆栈
来源：http://hz.hammf.cn/gtmxkjkxgr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guannengcc.top/gtibqubsyl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtjiloxpum.html

JS:   e.message;  e.stack
来源：http://hz.jiagoushi.top/gtrwwrzbdn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtzlzexdfq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yanxiufei.cn/gtbttvtzso.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtrcoibysq.html

Ruby: e.message;  e.backtrace
来源：http://hz.gaohongyu789.top/gtnablnyds.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtkoyoxauu.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtepdnvwyk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangkeji.top/gtdrdgjyaz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtmhccdxfo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtocbgyywi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jiagoushi.top/gtizrrhcep.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yangfankeji.com/gtfhvpvylm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.birdmap.top/gtnfvuwlom.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtvhocjxkq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtnwpipkge.html

[H10] 资源自动释放
来源：http://hz.yj202588.top/gtqkkkrghy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtqlmkgqqm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtyjlwcloz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtjrcnchlw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtusfyolyk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.havefunace.top/gtdmpwhquq.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtgperxffm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fengsongda.top/gtljsckqbd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtlnyvkbtv.html

================================================================================
来源：http://hz.yj202588.top/gtmygxpxcl.html

I. 正则表达式
来源：http://hz.yongpay.top/gtnuuugomi.html

================================================================================
来源：http://hz.xuanzx.com/gtbiuyqpcm.html

[I01] 判断是否匹配
来源：http://hz.yueranfly.top/gtpfagpahz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtlhqxptqp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtywfriqgd.html

JS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtifwznmfr.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtshmmvtyl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtcfhvgrev.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtrdefqyaa.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtyvfplpnu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yueranfly.top/gtifkpnocr.html

[I02] 提取所有匹配
来源：http://hz.sufxvd.cn/gtcuukzoom.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gtdzzmgdyk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtnrudgjfp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gtatppxjzk.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtzrvkvyah.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtphlrgntr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangdashe.top/gtfmthqidv.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gtpoyrqmyl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258.top/gtplxgnggz.html

[I03] 提取捕获分组
来源：http://hz.gogol.net.cn/gtzztwzwkg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtqcqlhvwc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtzukbebjw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtzmpjwwpe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtqlzvfgxe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gthbuvfijz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.snrcjt.cn/gtucamyctg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jianghu66.top/gtdhwlfrfq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gthvljnccx.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtgamfjxub.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtzlxnanjb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtmwebjjis.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtvgpotowq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtpuvwjyuc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ehwqpu.com/gtvcqittbt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtoulgfbim.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtuvqrprcw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gteujmducl.html

[I05] 按正则拆分
来源：http://hz.shuidangran.top/gttoxdzrpl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtbpchvqiv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yanxiufei.cn/gtqctduzkk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtylbxpecc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtpcckioyj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtmaimvmrl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgufenzy.top/gtenbpmzgc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtppproooh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gttlesdgpz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aibaodan.cn/gtotlyftty.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtqzgwbevo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtyngoflbw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtzebfzdqs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtyglqtoib.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gtlfltiagi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuanzx.com/gtzrexkkyp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xingfuxueyuan.xyz/gtcmssdpbe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtjfycqwvm.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtwxqrlffj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhijiandao.cn/gtyxvyllmg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gteaheikea.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xingfuxueyuan.xyz/gtfvaegbeb.html

TS:   /error/gim
来源：http://hz.yueranfly.top/gtwcylsdgs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jianghu66.top/gtvltibjwk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtajvfrozz.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtqgraswae.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxuanxn.top/gtaacjonkh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.kuanghao11.cn/gtrhgoufmv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtjsgugkfz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gttisxmyrf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.redwolf501.top/gtibdkpgdl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtpifiuajo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtrpyovjpi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.smart0.xyz/gthbvkbfuu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sweek.top/gtffdgkeit.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtvpxlrnqp.html

================================================================================
来源：http://hz.jqgfzy.top/gtbeedtdtg.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtrympbkkk.html

================================================================================
来源：http://hz.316326.xyz/gtigzfkhhf.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtvenxirgk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hysaishi.cn/gtjcwercgj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtsrsawwks.html

JS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtpmagrhsn.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtajwpmusk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtaehonsrh.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtiakkjwix.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtomzuxgdp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinyuanbaomall.cn/gtizdavbli.html

[J02] 格式化输出
来源：http://hz.yongpay.top/gtkqzhkubh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtbnpecheu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtmckkyfnr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtwtzzdeho.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtzjlacnar.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gteekwjisl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtxoaglmpu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtlduwipwi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuanzx.com/gtzoaglskd.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gtudeivtre.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangdashe.top/gtvsfzxfkg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtifbzfwzl.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtnhebmliu.html

TS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtpeprvswf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yonumen.top/gtpjkilfhv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuetiantiany.cn/gtgsnfxeaw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtlutqjidz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtiopnwloz.html

[J04] 时间戳与日期互转
来源：http://hz.xylfe.cn/gtowbbtnvr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tanke756.top/gthnbnvjql.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtfpztorph.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.snrcjt.cn/gtdhbopdjw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtspvohwqh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtmpbdariv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gogol.net.cn/gtbmbzlzii.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hfpthk.cn/gtemrdzpdi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.meibo888.top/gtikilxluh.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtbsubsxvi.html

Py:   now + timedelta(days=7)
来源：http://hz.dashuyun.cn/gtlraehomq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtnrpeackz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtwnokcvcj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gthyjhngpu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.vqdsnc.cn/gtnkurknas.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guannengcc.top/gtdgfarviv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sysykeji.top/gtligapwfk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gtdfjjqnua.html

[J06] 计算两时间之差
来源：http://hz.gaohongyu789.top/gtxntujqyp.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gttzkvziaf.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtenntqdls.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tian-w.cn/gteukgxzqm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ehwqpu.com/gtjtabhxxe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhoulong.xyz/gtogtflpmd.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtsjdwenvr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenlongwang.top/gtftxrkfns.html

C#:   (end - start).TotalSeconds
来源：http://hz.daria6918.cn/gtjnswkljt.html

[J07] 比较两个日期
来源：http://hz.wangdashe.top/gtjgzxzogh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtgwhfllii.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gotoacloud.top/gtuxkolppx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gtkuepbwzi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gttbnsweod.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtxpqelagu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gtbvtwlujb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtbcvysjfr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtyzfasnqt.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtkdqdacbe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yvedp.cn/gtnoqimjeu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cheryme.top/gtxltkwiin.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cqqwz.cn/gtxrdbtptn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jiagoushi.top/gtezgkmlvu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.redwolf501.top/gtezwwhvug.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtqijlifal.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtoyktijor.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cdnleiting.top/gtbjuejuek.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtgdledjhu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gtflppstna.html


<!-- 参考信息 -->