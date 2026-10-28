代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.shangyingyoupin.top/gtopsvqguw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtoxecgyes.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tianlin.xyz/gtozuckljj.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtdbpjdows.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtiyysasbn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtxszztejs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtozubthrq.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtjwiurofx.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gtnoeqoyze.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtqwvdrtru.html

PHP:  public / protected / private
来源：http://hz.chenlongwang.top/gtdgaskjtp.html

JS:   #private 字段；其余公开
来源：http://hz.sufxvd.cn/gtwlzqedjx.html

TS:   public / protected / private
来源：http://hz.guowangkeji.top/gtrsyxamrv.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtnqfoeaed.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtkriokrwn.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gtijnuvmdg.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtmphzyoxx.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtkvteahms.html

Py:   @property 与 @x.setter
来源：http://hz.jqgfzy.top/gtevsrbjra.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.havefunace.top/gtnwhjlqph.html

JS:   get name() { return this._name; }
来源：http://hz.sysykeji.top/gthpkdwphn.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258888.top/gtvemkliub.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtmrrrnwfh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.smart0.xyz/gtriomlpeb.html

Ruby: attr_accessor :name
来源：http://hz.hnxiangtu.top/gticvbyqdy.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtjncxlcjk.html

[G12] 对象转字符串
来源：http://hz.yuxming.cn/gtolurawwh.html

Py:   def __str__(self): return self.name
来源：http://hz.ivvv.top/gtlxnfjddr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtytucgzbx.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gtqmloaxwk.html

TS:   toString(): string { return this.name; }
来源：http://hz.fengsongda.top/gtfywcymaz.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gthvayomol.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gtmayithna.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtgrshmngw.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtfitxeiiy.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gtwpbebtqs.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtoexwkday.html

PHP:  $u instanceof User
来源：http://hz.bjfxy.top/gtvasthhsc.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gtnxotdwex.html

TS:   u instanceof User
来源：http://hz.52xcode.cn/gttmneulps.html

Java: u instanceof User
来源：http://hz.svipenyu.cn/gtpoytxngq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gtvqfkoied.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gtivdsltlk.html

C#:   u is User
来源：http://hz.jinghuilouyu.cn/gtznvojrnm.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtvpbmjfae.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtbvrbhije.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.haohaochexian.top/gtvezajxcb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.c1oappe.top/gttqisgiem.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxuanxn.top/gttmfoqace.html

Java: record User(String name, int age) {}
来源：http://hz.haohaochexian.top/gtqamrhvzo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.snrcjt.cn/gtzjujfghj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hfpthk.cn/gtmihqknrd.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtlzwhyctb.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gtvhgegesh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cdnleiting.top/gtowzjgvrt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinyuanbaomall.cn/gtkuphbemb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtuyqthmry.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtiettenks.html

Java: enum Color { RED, GREEN }
来源：http://hz.aizwys.cn/gtqoxtlhax.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fengsongda.top/gtrxgwvzwy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtpvovouil.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtfeodatfm.html

[G16] 对象转数组 / 字典
来源：http://hz.dashuyun.cn/gtgiydrmgi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtlvrgijke.html

PHP:  get_object_vars($obj);
来源：http://hz.jyoumei.cn/gtenumkecf.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtlblfbesg.html

TS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtusjpkyvc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtnxpoikic.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuxming.cn/gtgxagoowq.html

Ruby: obj.instance_variables
来源：http://hz.0kj1m.cn/gtnxfsmcvd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtnunbwhgo.html

================================================================================
来源：http://hz.ivvv.top/gtkleoqnof.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtzwowwrqg.html

================================================================================
来源：http://hz.hysaishi.cn/gtboikjihe.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gtnvxvprit.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shangyingyoupin.top/gtpaczoywa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aizwys.cn/gthusqkeuk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtgqgjjdmu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtsglyjglx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtkcyyrdir.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yangfankeji.com/gtizaopeks.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gtttcradeh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tanke756.top/gtnrzxqlvs.html

[H02] finally / ensure 收尾
来源：http://hz.vqdsnc.cn/gtfwyxnodq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtwcuqypxh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtvqfzyrlm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtoonhtvxr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtpucnvehc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtvkgqglbg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daxiang520.top/gtlxejjsub.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtosdsafiv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gthmeaqsvs.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gthxfmsptc.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhiwuduotai.top/gtflhtomsc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtjfzrcyhi.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtdbykgzxl.html

TS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gttdhslptc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtiystffos.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daxiang520.top/gtgxcckplz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtmvgatajk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtfinadkoq.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtqbfiqscu.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtdsbncccn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtkybhxbkq.html

JS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtnntbjnqa.html

TS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gthqgcftfw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtojlbfiip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nwbrower.top/gtirqqmknl.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtxjuovhyg.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtvcvlmzbd.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtehmndjdt.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gtzduvphcy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtgtgvqzdz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtbcszaqed.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtlpxqosly.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuetiantiany.cn/gtseezfaby.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtduupcgmv.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigfzy.top/gtmdodsehx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gtunfywkbm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhixingplan.top/gtailfsdjx.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtlzijuuqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yanxiufei.cn/gtoxtnzhun.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtmgqybggl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtjkuwqpcs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xinyue.icu/gtssibrvqz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtoikcwdgn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gtfkhckdgw.html

C#:   obj?.A?.B ?? default
来源：http://hz.iojbl.cn/gtxmozccrz.html

[H07] 断言
来源：http://hz.hfpthk.cn/gtzoovyyqy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.feifeiyinyue.top/gtwdeemtrz.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtcodifyua.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtmereiajm.html

TS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtntkeoadf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daria6918.cn/gtbdqaxhxw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtdeoygtzt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtqgvpusjf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtsokmuvhi.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtzjrxuhan.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtnbxuwolt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shangyingyoupin.top/gtmiuadkwo.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gthozlrbxz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hfpthk.cn/gthyklhqwu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtxwcohiog.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtehhhuflg.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtwatzaqqj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtmqncxrfs.html

[H09] 带错误码的异常
来源：http://hz.gotoacloud.top/gtemjunfpo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yvedp.cn/gtkmjbskga.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shangyingyoupin.top/gtfeyrpwhg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gtfqmglbuq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtuuynhmus.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daxiang520.top/gtchjudaps.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gtucbattsj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtscprcevw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtazmxxvkk.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtxortzevh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtquvgkgup.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gtxqestyyc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gttsuvqqav.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtuhkflgrv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gtymtnhfnw.html

Go:   defer f.Close()
来源：http://hz.vqdsnc.cn/gtrctogvfn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhixingplan.top/gttfluocje.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtazoujson.html

================================================================================
来源：http://hz.zhengqikj.top/gtwwoepvog.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gtfaazgxtj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtkcqhpqss.html

[I01] 判断是否匹配
来源：http://hz.jinyuanbaomall.cn/gtzxmjenwy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tianlin.xyz/gtiptsknwm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtoidzispz.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtpkuacodb.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtnhhbywoi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gtvfyehuzf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtizfyzmpt.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gthzelruor.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtizehqigk.html

[I02] 提取所有匹配
来源：http://hz.zhoulong.xyz/gtaikizbqp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtoiuwejci.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgufenzy.top/gtfdqtucpm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtittclmbf.html

TS:   s.match(/\d+/g)
来源：http://hz.yongpay.top/gtlufldkbl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtmlhiihzu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtnbbfkqqg.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtzenuirbt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gtkjuqoalm.html

[I03] 提取捕获分组
来源：http://hz.cashguo.top/gtxqgkqmph.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtmsbyfqcp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtiitjpjhb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tanke756.top/gtyvduvauh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnqzz.top/gtuxbkoodt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gtxafjbatx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenlongwang.top/gtxpsuvinz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtemdnxora.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigufen.top/gtysisygxl.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtixvfumze.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xziqi.cn/gtaoxujpbk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gtabyqkyve.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtnvudaguf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtwbdyqhqp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhixingplan.top/gtqmjoyeyz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gttwjwylmg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtldwkilmk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shangyingyoupin.top/gtizhhrach.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtjleunpww.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtdasnfgmb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gogol.net.cn/gtfeqcdhfg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtvabpfuzm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtxzbjkzyk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtdhwrpjif.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj202588.top/gtufqgkuyz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtrihzmbpc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tian-w.cn/gtwmhelhre.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gttaojuykp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtuutkszsp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtfqzsqfgj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gttdadyssv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtxdnirhju.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.quarkkingdee.top/gtianxatqo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhengqikj.top/gtvftcfnsu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtosthrgjc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtxangmdjf.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtvotvmwim.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ywan-chungtsiang.top/gtohsacenb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtigbetyhs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gtckffibff.html

TS:   /error/gim
来源：http://hz.hfpthk.cn/gthetiocvc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hywenlv.cn/gtmwvbdmyn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtfnzcibax.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtkxxrilev.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtsdbprqkh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.snrcjt.cn/gtscledcdo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtceyvuyha.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtsfpufjoc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtezltrxkb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtinnvemcr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtjwwnqadq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cqqwz.cn/gtdofuddfu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtncadplgn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtneaomowu.html

================================================================================
来源：http://hz.nanxuanxn.top/gtitfghdod.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtyamfippc.html

================================================================================
来源：http://hz.yuxming.cn/gtjydglytb.html

[J01] 获取当前时间
来源：http://hz.shzxlz.cn/gtbiqmammn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.quarkkingdee.top/gtoembzyqc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtjwifefiz.html

JS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtjkmrlqww.html

TS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtwbrqtxod.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtxdglnkuq.html

Go:   time.Now()
来源：http://hz.shangyingyoupin.top/gtriqfywbh.html

Ruby: Time.now
来源：http://hz.zhaomingkeji.xyz/gttkyeeqmw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.birdmap.top/gtyzuupxzs.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtalhcxqtu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gthbfmyiyr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtzvikoury.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtlgvigomo.html

TS:   d.toISOString()
来源：http://hz.cheryme.top/gthfxnzywq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtnxywxijl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtulizvutw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtknnogzyb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.svipenyu.cn/gthwuczwpc.html

[J03] 字符串解析为日期
来源：http://hz.zhijiandao.cn/gtfznioyxu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.feifeiyinyue.top/gtwaplqrwo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtysyhmcwz.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtwahegpey.html

TS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtgtsafjbr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtntpsphnv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gthqnkeapa.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtgsmebqyu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aizwys.cn/gtanhgeinw.html

[J04] 时间戳与日期互转
来源：http://hz.jinghuilouyu.cn/gtgvtcdzbz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ehwqpu.com/gtfvgvlvhz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtaqapnikx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gtzbxcvrpw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ppjwa.cn/gthllohirs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtpyetqtuu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtqnqmfzpu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinghuilouyu.cn/gtsymzjrkf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtbuqqklbp.html

[J05] 时间加减（加 7 天）
来源：http://hz.hysaishi.cn/gtdtkctlza.html

Py:   now + timedelta(days=7)
来源：http://hz.dianchejie.cn/gtdphmwsku.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtwwqgwgqk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtkjtdwoxr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtytbzcczi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gthccpxzqw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtcsieewor.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtizrsluqa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.iojbl.cn/gtwemwuxaa.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtjgezuqsf.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtizdbdsgn.html

PHP:  $end->diff($start)->days;
来源：http://hz.cdnleiting.top/gtccsuzuqu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gzhubu.top/gtrdvvlbud.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ybcxt.top/gtuhzeidid.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgfzy.top/gttlmwcpoi.html

Go:   end.Sub(start).Hours()
来源：http://hz.guowangkeji.top/gtihuylqns.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gtwbsoeimq.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gtbmplzygi.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtdejbxokf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtpojcluzt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtulzjcwoo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtcrvnfrro.html


<!-- 参考信息 -->