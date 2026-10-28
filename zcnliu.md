代发 wailian999

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtzzbmrzzc.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxuanxn.top/gtmblejhpg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtcpvkqpzw.html

Ruby: public / protected / private
来源：http://hz.svipenyu.cn/gtmgzlwyel.html

C#:   public / protected / private / internal
来源：http://hz.316326.xyz/gtnyqzhtqk.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gtgajxaccm.html

Py:   @property 与 @x.setter
来源：http://hz.shzxlz.cn/gtibhmslja.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtwekwponp.html

JS:   get name() { return this._name; }
来源：http://hz.jlsjyb.cn/gtvdupidnx.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gtkmywwyzc.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtxdsttyrf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tanke756.top/gtsxlbiynh.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtfivgvyip.html

C#:   public string Name { get; set; }
来源：http://hz.ybcxt.top/gteuymsqgl.html

[G12] 对象转字符串
来源：http://hz.jiagoushi.top/gtuuksrgac.html

Py:   def __str__(self): return self.name
来源：http://hz.sysykeji.top/gtjybntdbf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtthcxmqrn.html

JS:   toString() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtdywjwatd.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtnexwlcnn.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtdocjtoft.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtngkokvhu.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtyqphpqdc.html

C#:   public override string ToString() => Name;
来源：http://hz.zhixingplan.top/gtzfvxuhmb.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtutnylyde.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtvwmrrwiu.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gtwnnrehal.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtofbhmvtu.html

TS:   u instanceof User
来源：http://hz.ehwqpu.com/gtqdyempvd.html

Java: u instanceof User
来源：http://hz.shzxlz.cn/gtvirornoj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtnxwldheb.html

Ruby: u.is_a?(User)
来源：http://hz.jqgfzy.top/gtneacpcpl.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtdgxqsprc.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtueirkcnf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daria6918.cn/gtvxsigcsa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xingfuxueyuan.xyz/gtqhtzdhsi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtzekwhknx.html

TS:   type User = { name: string; age: number };
来源：http://hz.cucudq.cn/gtxwsjchjs.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gtfnflhfzs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hongshengwenyu.top/gtrwzbsjeg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.haohaochexian.top/gtpubpuczd.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtzswufzut.html

[G15] 枚举
来源：http://hz.sxryk.cn/gtkufvgbrc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gttqphyjyq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gtakjoidvn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtgxnuikkj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtitzkwtqw.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtfytgqfii.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gtwlaivksm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtupdxemey.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtmkomvuiz.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gttgbqsdze.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yvedp.cn/gtjfnhwkvf.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtfytwaknd.html

JS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gttvhzdecd.html

TS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtusflzxcd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtqyhbcqdk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtgzzgwjgp.html

Ruby: obj.instance_variables
来源：http://hz.gotoacloud.top/gtiympfpkz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtujgnjqau.html

================================================================================
来源：http://hz.zhijiandao.cn/gterktrgqi.html

H. 异常与错误处理
来源：http://hz.316326.xyz/gtpcslakho.html

================================================================================
来源：http://hz.svipenyu.cn/gtlpbmovnj.html

[H01] try / catch 基础
来源：http://hz.haohaochexian.top/gtwucvfofe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shzxlz.cn/gtgcbeafyv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtomilcswb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtregjchmu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtfznbvgiw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pengpengdd.cyou/gtowcjsuum.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhijiandao.cn/gtgjtnmntb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtvtmlfcft.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.0kj1m.cn/gtbujynzqw.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gttunyisex.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtziyhmigs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtutuoujic.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtgsfgeaee.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtqwmcaevs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtedrgouuz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtawyfranb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtfvtgfmtu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sysykeji.top/gtofqimtto.html

[H03] 主动抛出异常
来源：http://hz.gogol.net.cn/gtclfbrtiq.html

Py:   raise ValueError("错误信息")
来源：http://hz.tian-w.cn/gtekuembgn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtgzhjdbvn.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtlhovypkn.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtubivgxqx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtllwhlrdl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gttbcpvayq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtzmuvuijd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtpkkvrzlt.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtawqdiiuf.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtjegtvouy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtxwwtgcna.html

JS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtityrbewb.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtxybqqolx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guannengcc.top/gtxhvvldnl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.meibo888.top/gtlttetykc.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtiofaggrn.html

C#:   class MyException : Exception {}
来源：http://hz.ybcxt.top/gtyodjfnwo.html

[H05] 捕获特定类型
来源：http://hz.gaohongyu789.top/gtncyvdgog.html

Py:   except ValueError as e:
来源：http://hz.fengsongda.top/gthtqwfwlv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.c1oappe.top/gtykldwnep.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtwtvgldhi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtwonhjdif.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.snrcjt.cn/gtfkcxonrs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gtvgbnqqjc.html

Ruby: rescue ArgumentError => e
来源：http://hz.9152youxi.cn/gtgmpjkprw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtjxipoxyq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtrawpowbj.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gticzhtpna.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtiqfrglxd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gttoxfteca.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtpfrquwli.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtmarmymxo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jianghu66.top/gtijpdvdyr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtxatienmi.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtcqiqoobb.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gtzfqanosi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtrjyssuld.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtsvzroyzi.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtnsknvqub.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtqxbaibpe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtkwijqiqy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gtdfttqmee.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangshuangyany.cn/gtpwfptusw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gogol.net.cn/gtnfltjztw.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhoulong.xyz/gtbhuoliau.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gtbytljxlr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dashuyun.cn/gtvfvngwaw.html

JS:   e.message;  e.stack
来源：http://hz.shuidangran.top/gtdxwllqtd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gttwdyfzwg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtecbcecns.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtinxxyvto.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtvzydbcku.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gtugscyxpj.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gtxhvfcacm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yonumen.top/gtcadhaooq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtrlxjqxuq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sweek.top/gtmgyjjujm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtwqectcjm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.svipenyu.cn/gtfrazkdlj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtvjhbgzjf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtfaggwhwb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gogol.net.cn/gtsftspghu.html

[H10] 资源自动释放
来源：http://hz.yuxming.cn/gthtgbwogd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtrfwokvju.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yvedp.cn/gtbihpfaal.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtltcihimn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtqmbyfrop.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxuanxn.top/gtsmthxbgg.html

Go:   defer f.Close()
来源：http://hz.mhx1999.top/gtpxhfqtlg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtcmgezqzs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtyzbnaxxb.html

================================================================================
来源：http://hz.haohaochexian.top/gtajmypzfo.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtwxprwdqv.html

================================================================================
来源：http://hz.zhengqikj.top/gtvkiwrshw.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtkehvzmgg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ppjwa.cn/gtklrzryue.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtqmcafyqa.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtkwxqrflr.html

TS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtkgfsjmjz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtwluyvxgp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtdqtiwtqt.html

Ruby: s.match?(/\d+/)
来源：http://hz.jyoumei.cn/gtupfvgwxq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtofcwyafn.html

[I02] 提取所有匹配
来源：http://hz.ehwqpu.com/gtwcburwtk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gzhubu.top/gtqouwgdpd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtejkfntdt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtzmiepexr.html

TS:   s.match(/\d+/g)
来源：http://hz.c1oappe.top/gtsimnvxon.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ywan-chungtsiang.top/gtzvsezwwq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtxvqfehao.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gtbqozapxd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtglgnfgqw.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gthmgfgxgz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtwtrepjhx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtjauxgulh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gthxuktpeh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gtsnbecivs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yvedp.cn/gthdodxxqs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gttjoovcak.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dianchejie.cn/gtraombtoa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xingfuxueyuan.xyz/gtjxesnzat.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtimqlyokg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhijiandao.cn/gtozgejnbl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gtnrckeadf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtyvcgjekg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtsgqwchdm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxuanxn.top/gtmjetdxeo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtowbjzjdw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gtihefvjrc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtwkkpevym.html

[I05] 按正则拆分
来源：http://hz.hongshengwenyu.top/gtmaxshvcu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtkuqtvmtk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtupaoppsv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtemnnpamh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtxdwybonp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dianchejie.cn/gtuvvopmnt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtedienyha.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtdzjxyxde.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtoikpgszz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtmlfnxtvo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtepgruizh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ivvv.top/gtvfyxocoy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gticdiregh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtzilfynde.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtxeoggcqg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yangfankeji.com/gtnihamusb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuxming.cn/gtznrseksj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxuanxn.top/gtgulqlwyj.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtisizliue.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.havefunace.top/gtkpptgblt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtwdnxvdbz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shzxlz.cn/gtprmacjxu.html

TS:   /error/gim
来源：http://hz.hywenlv.cn/gtkebjiahy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gthpetktgn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.snrcjt.cn/gtyszcauty.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtuqbqkbpk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hfpthk.cn/gtdqflngfi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtsdrubfdg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnxiangtu.top/gtimxsobjq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtdfffpyvx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtlnmhfbvn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtdmvziasr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtmrxabnrc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sufxvd.cn/gtccrirgep.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tanke756.top/gtpigxnvof.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtmykenphk.html

================================================================================
来源：http://hz.sweek.top/gtwsihetbd.html

J. 日期与时间
来源：http://hz.zhixingplan.top/gtplussvkt.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtsbmhlxyr.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtdnmbsnob.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gtddyqymoz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtgpbrbpfn.html

JS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtjhyotdat.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtcunplgpr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pengpengdd.cyou/gtylqvczjw.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtvwtnsxbs.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gtzobtlboj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtlbtioaqm.html

[J02] 格式化输出
来源：http://hz.zhijiandao.cn/gtnuxxpdsk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtwaswfqgr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtvnqiymdz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ywan-chungtsiang.top/gtmpnwaqkz.html

TS:   d.toISOString()
来源：http://hz.dianchejie.cn/gtyaybujpk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gthqpbcuft.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sxryk.cn/gtbngvznht.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtbbgfecqe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtjpcbducn.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtjvmsqsvx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dianchejie.cn/gthmbuheax.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gtejmwzgkp.html

JS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtkijcqzfh.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtzxeujogw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gthgziizyi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtyqskutln.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtjybxdpre.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.0kj1m.cn/gtbzdmtwzu.html

[J04] 时间戳与日期互转
来源：http://hz.0kj1m.cn/gtzffhknhz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hfpthk.cn/gtmexnyrtg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.meibo888.top/gtlzqoqgxq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtwpurkxad.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtueokgzfq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gtaskzxnmh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtyrqduwzd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cqqwz.cn/gtszxsleyc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtisauyfjp.html

[J05] 时间加减（加 7 天）
来源：http://hz.kuanghao11.cn/gtrzqkbesv.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtinuwclbz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtheafdwiz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtwsandedd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtgqagzgcg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.vqdsnc.cn/gtgtkjclhz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yvedp.cn/gtyzhegots.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gttohwafad.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtmryuwktd.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtwlrrzprt.html

Py:   (end - start).total_seconds()
来源：http://hz.guannengcc.top/gtdlbremea.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtrwrpxbge.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yangfankeji.com/gtvrcgyxsp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtyghskhkb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangtech.top/gtciitynyw.html

Go:   end.Sub(start).Hours()
来源：http://hz.jlsjyb.cn/gtaocujgbt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtxmzqkzzi.html

C#:   (end - start).TotalSeconds
来源：http://hz.svipenyu.cn/gtkocnintt.html

[J07] 比较两个日期
来源：http://hz.gzhubu.top/gtzvvnqfqy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtyessbgdr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtouvwjyro.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtdtmeuwmx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtzmjlgaug.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.0kj1m.cn/gtdlmgbztc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pycfn.com/gtyezznfnc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtuccwobvo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtebhraswa.html

[J08] 提取年月日与星期
来源：http://hz.shuidangran.top/gtdsxzvntw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtyyrkgxho.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtyoifmbwu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtnwoxrevw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tianlin.xyz/gtjdmvkbfc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtmabyazpi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yvedp.cn/gtwyqlzxpj.html


<!-- 参考信息 -->