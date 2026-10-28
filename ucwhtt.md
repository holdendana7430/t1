代发 wailian999

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtlgpeunts.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtwkrhbdkz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtqelqpgld.html

Ruby: public / protected / private
来源：http://hz.birdmap.top/gtxowqpsaa.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtsaowcuwg.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gtavwtrigm.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtsuzldycp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtgyhxxjzb.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtyjdhuclb.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gtxtxyvzwn.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gthsahmfnn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.snrcjt.cn/gtynulslto.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangkeji.top/gtaryihunh.html

C#:   public string Name { get; set; }
来源：http://hz.xuanzx.com/gtkanvhpkx.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtigpgcgvn.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gtovjtgtle.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj202588.top/gtzsplikvj.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtdqzbvpum.html

TS:   toString(): string { return this.name; }
来源：http://hz.shuidangran.top/gtgkkrrftz.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtyrcohnoo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.0kj1m.cn/gthlzrexjq.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gthbbowsal.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtxgloyekq.html

[G13] 判断对象类型
来源：http://hz.nanxinkj.top/gtlnqthneg.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtmsvvjsnu.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gtjiebrxff.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gtmqzsxhol.html

TS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtuzszesfg.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtpbdzyogk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtmqemoska.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gtdmiypuot.html

C#:   u is User
来源：http://hz.xziqi.cn/gtnqdzjvxw.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtifjueyjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtbvejhjqs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gthttexyjx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinghuilouyu.cn/gtrmiktnjw.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtpdfqwjbx.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gthojomwma.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtgakdjqik.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtkxsmgiyu.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gtzhnyoobe.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gtbnvfnbbh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtwytjgrxy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sufxvd.cn/gtqeiowbdv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ivvv.top/gtewotxgkv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtfeaghdua.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gtrizebteo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.0kj1m.cn/gtmtzfweyi.html

Ruby: Color = %i[red green].freeze
来源：http://hz.quarkkingdee.top/gtldwcwhbk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtfxcuiqqb.html

[G16] 对象转数组 / 字典
来源：http://hz.shangyingyoupin.top/gtfacfpezu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xziqi.cn/gtvhsjxhka.html

PHP:  get_object_vars($obj);
来源：http://hz.xuetiantiany.cn/gtaausyjuw.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtxjapfrbp.html

TS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gttkdxhfpo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gthwlmglgp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gogol.net.cn/gtukhugiiz.html

Ruby: obj.instance_variables
来源：http://hz.nwbrower.top/gtpjdwdjmg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtakshpwad.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gteryuahig.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtdgwfgrbm.html

================================================================================
来源：http://hz.0kj1m.cn/gtxchavaol.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gtoldnnzip.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.smart0.xyz/gtcreezauy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtnvotztpa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtjpsmkoby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zdqjudy.top/gtlkkoivog.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xingfuxueyuan.xyz/gtgppliwbr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtoqqmqyuh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.snrcjt.cn/gtlregnbuq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhengqikj.top/gtbzeeirdh.html

[H02] finally / ensure 收尾
来源：http://hz.zhixingplan.top/gtbasbdeie.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtibeitoly.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gteumwabiu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtelsvowxm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtgbmscmwe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gteibwpgcw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtxqscqgdo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtkirsqily.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtfzrbtygq.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gtobvoswda.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtalzyxcxl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtovvhtviw.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtlddcgrpy.html

TS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtclaenitz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pycfn.com/gtzegvzvvs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtrojcylop.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.vqdsnc.cn/gtzlyddjpj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtlnwycefr.html

[H04] 自定义异常类型
来源：http://hz.yongpay.top/gtiuvrockb.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtpdtbjuwj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtbbrzypep.html

JS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtzxpnaztj.html

TS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtmcokhnyj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtyxdmznes.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtgweuyopa.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxuanxn.top/gtdpfpifmc.html

C#:   class MyException : Exception {}
来源：http://hz.quarkkingdee.top/gtysbeanbo.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtzzmglyma.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtkkzyhbha.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.vqdsnc.cn/gttkovultj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtfcwtejsl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gteydrcjcf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gtfbyhcysb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinghuilouyu.cn/gthexuwcdx.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtjtckvsmb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.316326.xyz/gtlvxsbxca.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtckegpebk.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtqcnhzemp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenzaomai.com/gtapbzkmib.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtazvyhqxt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtbrrucxjq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yanxiufei.cn/gtucygfivp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgufenzy.top/gtptizcziu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.bjfxy.top/gtyuguczkq.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtywwtrlqt.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtihpayyyd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuetiantiany.cn/gtnfjwhoas.html

PHP:  assert($x > 0);
来源：http://hz.nanxinkj.top/gtswrtsasn.html

JS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtsjmkcxnk.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gthtvvzvvo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtnerjkbnl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydzc1.top/gtdkqotere.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtpmlacyyk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.meibo888.top/gtjwzlavne.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtfpjiubrg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtfvodijux.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gtswoqpjix.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtstgcvsmn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtsrhibueu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtffybxmlm.html

Go:   err.Error()
来源：http://hz.hammf.cn/gtqovsdhat.html

Ruby: e.message;  e.backtrace
来源：http://hz.xylfe.cn/gtpwkexpeg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gtmhauljya.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtnaevwqnd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hywenlv.cn/gtwsvngyiu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtmyvsszmj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hfpthk.cn/gtzwzmcxyi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtcpqguesb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtndcdgoyb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sysykeji.top/gtbqbsupoh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hongshengwenyu.top/gtfoboklvm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtspqixgts.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtlwuicvpv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtaxaofbhs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangdashe.top/gtsgxnyzwu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtusqrbqvo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtqkelblsf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtjtvmiwfq.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtgwelgkhk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtoshopnwr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shangyingyoupin.top/gthtfvlitt.html

================================================================================
来源：http://hz.mhx1999.top/gtmljjhvkr.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gthsjazxwu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjwqwlrve.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtgmqqihrd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtryvaxbuu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtcecxhztj.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtmifxgkzg.html

TS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtyjubvhlx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtbtrnzmwe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gteqzrzvnb.html

Ruby: s.match?(/\d+/)
来源：http://hz.cqqwz.cn/gtkqgwuikz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgufenzy.top/gtvosjraug.html

[I02] 提取所有匹配
来源：http://hz.gaohongyu789.top/gtqbnrgqwl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenlongwang.top/gtcjamruom.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtiwiujbao.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtzwvhmkbr.html

TS:   s.match(/\d+/g)
来源：http://hz.jyoumei.cn/gtwvsyzkhj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.redwolf501.top/gtipyntiba.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtifesgpwf.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtwjhxtlgn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxuanxn.top/gtajtovjpl.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtxsjyajbo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtlgavhbbw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuanzhike.top/gtdgtfhjwj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtgxyigccd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinghuilouyu.cn/gtuuxyzhql.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ybcxt.top/gtylmxbspq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shangyingyoupin.top/gtnmlvrkcd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtygwdluux.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtmdtdhqgc.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtmfvgmrpc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zycfv.cn/gtyphulwnk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gturzyvuuw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtmolzgjdk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtshvkcqyv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtbfalqtsz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtbaeosggi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtsdgmytgt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.svipenyu.cn/gtrboovqwo.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtwpddfkdm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nwbrower.top/gtipvkabxv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydjk.org.cn/gtjdrowleg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtwylrzhjj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtxmltjzrd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhengqikj.top/gtxvomyxgk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtenbfbizg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtrjvrgbor.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daria6918.cn/gtgcovekkh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ywan-chungtsiang.top/gttpalgvrx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtfzslhfnb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gthshoaxks.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtmzzchlsz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gttgvdjzjc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtbkfiofkm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigufen.top/gtpxlljtbh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtjkvswilt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtnttabhnd.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtkhztxrgh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtkolueoyq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtbjfjqwlr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hysaishi.cn/gtuinxehmc.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtebqdhjiv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtlakkvtcb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtfmvvaaqn.html

Ruby: s.scan(/error/i)
来源：http://hz.hysaishi.cn/gtplvoddhs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangdashe.top/gtyfzkkoyv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cheryme.top/gtxvdoqktn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sufxvd.cn/gtqhdsqjqr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtdtqgnqlo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtbdhvnvvm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtustffqti.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtnottqdlv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tanke756.top/gtcjvedmwg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtglygfcwu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gtcluovtnd.html

================================================================================
来源：http://hz.cdnleiting.top/gtqgupjzhd.html

J. 日期与时间
来源：http://hz.aizwys.cn/gtzfrbovxi.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtrbkutufy.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtdnigeqmj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtyyjncqac.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtatzrbokw.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtrgltjhgl.html

TS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtbnbwnuvw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.haohaochexian.top/gtcpphksje.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtynubzcck.html

Ruby: Time.now
来源：http://hz.yj202588.top/gtckbflunm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.birdmap.top/gtxabxcjgr.html

[J02] 格式化输出
来源：http://hz.havefunace.top/gtullslanm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtybhlqzuh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtbflsyvbz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtnfkefebc.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtaoexyhtq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gtaoqjqmbq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtbvzmddiz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtkdpksues.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangtech.top/gttnwviudp.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtyalyssir.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fengsongda.top/gtehwwrcow.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxinkj.top/gtpekoeufz.html

JS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtitplthwo.html

TS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gttymzxggh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtxmrgufuh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cqqwz.cn/gtqgaxbdow.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtyjlykwcb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtsvtgzoez.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258888.top/gtmstjtcyo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gtmmpofjgs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtukuclohi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.wangdashe.top/gtkdvxumai.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhengqikj.top/gthaaoxijd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gttjoiwfjd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtwbeioukc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtndocqoyh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gogol.net.cn/gtsxdqmhav.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtqxyojmqo.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtbilhwaof.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtrsflqxtl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtagfpzuux.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtcmselkaj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gteutkhfwl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtvcsjtvhh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yueranfly.top/gtnbvszemv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.vqdsnc.cn/gtdpvzcdzq.html

[J06] 计算两时间之差
来源：http://hz.yueranfly.top/gtxevkutsv.html

Py:   (end - start).total_seconds()
来源：http://hz.gaohongyu789.top/gtaldrgeaj.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtfanriacf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtjuglfvwb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gtyquupbty.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtiulhnrba.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtjdcisyyk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtxpjwczaj.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuanzhike.top/gtpnumvhyp.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gtsmovmpoj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtdughbtds.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sxryk.cn/gtemzfhxgc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtbzdexvxt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtaolnypsu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtfxcqqgkr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cqqwz.cn/gtdkzeurti.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtmqjmibjn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtepucqdfd.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtlbpoaxyt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtfhqgzgro.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cucudq.cn/gtvvahktbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pycfn.com/gtpqdxbdjq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtrdjecxld.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtfambfrgj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gthxejwuoe.html


<!-- 参考信息 -->