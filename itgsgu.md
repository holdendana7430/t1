代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtjxdivhag.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtgeznkfbb.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gtejhuvddh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cheryme.top/gteycyvylv.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtpyrhwzyz.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gtipikvdfx.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gttycpowxd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtmxgdpkgz.html

Ruby: attr_accessor :name
来源：http://hz.daxiang520.top/gtqecfwhzc.html

C#:   public string Name { get; set; }
来源：http://hz.snrcjt.cn/gtqviklsqf.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gtvlzkywrz.html

Py:   def __str__(self): return self.name
来源：http://hz.gotoacloud.top/gtgwroqzoq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtpcaxmuyo.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtzniayxap.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtutkwiacw.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtzrijxgix.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gtzjuyrhag.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtgylywler.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtqzplmfee.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtbhhyvwwt.html

Py:   isinstance(u, User)
来源：http://hz.jinqigfzy.top/gthfedkges.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtvhwxfnql.html

JS:   u instanceof User
来源：http://hz.yongpay.top/gtzsmigidh.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtlunpiwlf.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtnvktenqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtjmisdhvu.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtxgybpczz.html

C#:   u is User
来源：http://hz.redwolf501.top/gtdsgjtrzm.html

[G14] 数据类 / record
来源：http://hz.cdnleiting.top/gthckjryoj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtwiriptfj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zycfv.cn/gtddiefdjw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtxqlwxwqv.html

TS:   type User = { name: string; age: number };
来源：http://hz.sxryk.cn/gtytijpvgc.html

Java: record User(String name, int age) {}
来源：http://hz.hnqzz.top/gtobrxxxyl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yvedp.cn/gtohkuthnk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gtkhxpxzyq.html

C#:   record User(string Name, int Age);
来源：http://hz.yvedp.cn/gtdinsalix.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtlzhgevej.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhaomingkeji.xyz/gttsjdggmr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hfpthk.cn/gtpbdzthxf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuanzhike.top/gtmsjiobnf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtskpvlzyn.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gtsugjiixt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuanzx.com/gtwtigwxtr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xinyue.icu/gtuounrlvl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtoeccebya.html

[G16] 对象转数组 / 字典
来源：http://hz.xziqi.cn/gtjmeqqqoc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtatwkeqwb.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtbctvtzwr.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtetntqovk.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtfduemswo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtdxyuvqij.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ivvv.top/gtjzffjlvf.html

Ruby: obj.instance_variables
来源：http://hz.quarkkingdee.top/gtczykiklr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtrnzbdfqa.html

================================================================================
来源：http://hz.sufxvd.cn/gtaccoscwu.html

H. 异常与错误处理
来源：http://hz.shuidangran.top/gtucemsrts.html

================================================================================
来源：http://hz.0kj1m.cn/gtasbmznnk.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gthjaynehf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtcshlupta.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.0kj1m.cn/gtakditcou.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtejsdaxrv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guowangkeji.top/gthzymmxof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtdwczejii.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pycfn.com/gtrdfqvzhz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gtwrculbep.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtlkrdodkc.html

[H02] finally / ensure 收尾
来源：http://hz.dashuyun.cn/gtmlnixqzq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtlckjbicv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtscvvfcyn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtfyyvxabx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtkcysrmal.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtdejewwgc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtgbufehue.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtavspfkke.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtzuyuldrh.html

[H03] 主动抛出异常
来源：http://hz.tianlin.xyz/gtauozjoez.html

Py:   raise ValueError("错误信息")
来源：http://hz.havefunace.top/gtaojjgmyy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtpxcnfwsw.html

JS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtwwjlzzqr.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtfdzfhbmh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtwkhlpcax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gtfbhrgwen.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yanxiufei.cn/gtgonclfbw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtahhqlmjz.html

[H04] 自定义异常类型
来源：http://hz.hnqzz.top/gthkspgkre.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gteofglopa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtlvrwqdcn.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtskapncrf.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtcdouyrqh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xinyue.icu/gtvpovlicl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtszwtmmql.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gtzgxhjiiq.html

C#:   class MyException : Exception {}
来源：http://hz.birdmap.top/gtovrblrrw.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtfwqbuclk.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtuqjrhbch.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtrxsilnjv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtxvcvltti.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtplvaphzz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtbujfnbam.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gtpbqadess.html

Ruby: rescue ArgumentError => e
来源：http://hz.kuanghao11.cn/gtqwihhwos.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jyoumei.cn/gtjzityhgu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hywenlv.cn/gtqephhxng.html

Py:   value = d.get("k") or default
来源：http://hz.xylfe.cn/gtbqzapywo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aizwys.cn/gtkgednioc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtsscjztnr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtjhwhpwky.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtbjqhqrsf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zycfv.cn/gtoppsqhog.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yangfankeji.com/gtscjbeiur.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gttsdxjmvo.html

[H07] 断言
来源：http://hz.jianghu66.top/gtotbvqpwc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gtwchuhshp.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangtech.top/gtllvnjthu.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gttkibrrwd.html

TS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtbwsxlher.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tian-w.cn/gtzlulyhgy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgfzy.top/gtfmzhswtx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtljpkzaqy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhijiandao.cn/gtrfjmavzr.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinyuanbaomall.cn/gtaxltlgyi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgfzy.top/gtfyqvdinj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigufen.top/gtsnctxtin.html

JS:   e.message;  e.stack
来源：http://hz.cdnleiting.top/gtxnuyqkey.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yangfankeji.com/gtcmwatxfn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtpkbliibx.html

Go:   err.Error()
来源：http://hz.gotoacloud.top/gtahqiymln.html

Ruby: e.message;  e.backtrace
来源：http://hz.jlsjyb.cn/gtolqcmpes.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gtsylptcka.html

[H09] 带错误码的异常
来源：http://hz.zhengqikj.top/gtdcsboofh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtisrjkntd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gtbvjozdfk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtbanajmbf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtebvuzgqh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtwqtmhisb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ivvv.top/gtybonfjqa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhiwuduotai.top/gtitskbqlc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.havefunace.top/gtjhfyaidy.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtpjczdnti.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gtqqyahamo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtmvvstixl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtqqvpwtaw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtwcvphltd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhixingplan.top/gtnelsmixj.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtujhecjxh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnxiangtu.top/gtzwxoupjy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtxpdxafjd.html

================================================================================
来源：http://hz.jianghu66.top/gthdkwgvrx.html

I. 正则表达式
来源：http://hz.gzhubu.top/gtncbpndvl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtejwuiufb.html

[I01] 判断是否匹配
来源：http://hz.hongshengwenyu.top/gtvcuxcwnc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gtpwbwbgua.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangtech.top/gtwbtvheag.html

JS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gttwozzaqs.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gthyyqtzei.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tanke756.top/gthpgovoza.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jianghu66.top/gtwfyagbwz.html

Ruby: s.match?(/\d+/)
来源：http://hz.svipenyu.cn/gtboocfclh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jianghu66.top/gtxwfrglss.html

[I02] 提取所有匹配
来源：http://hz.gaohongyu789.top/gtbjwyzaoz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtwzpasous.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnqzz.top/gtudmgdwop.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtzbyrzaay.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtcgrqxefc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtgrawiolv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.0kj1m.cn/gttyjfhbmc.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgfzy.top/gtzcnxkosu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigfzy.top/gtvsgqunyn.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gteokjtlss.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtmgoxqcty.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtvgesapfo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.iojbl.cn/gtsvnijdvn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtgtzuzetx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gttsenitwa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sweek.top/gthpdwilqh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtofenhwvg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtstnquyaj.html

[I04] 正则替换
来源：http://hz.sufxvd.cn/gtpdlqslfh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cheryme.top/gtftztetht.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtintnueou.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tianlin.xyz/gtfqpueytd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtwzsiygpb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtiiutdoxe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtwnuxoksq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.feifeiyinyue.top/gtfzljytyz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtsegtnngt.html

[I05] 按正则拆分
来源：http://hz.zhijiandao.cn/gtegilvqeg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtgrrcbyae.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydzc1.top/gtjrmrhasv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtklikxzwl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtrjmlrvyr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yvedp.cn/gtzwacfelt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtrxanqvly.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtbgwfnylw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtrehlbxyf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ivvv.top/gtjvpvzmne.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtrkrbfspv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgufenzy.top/gtuhucpaqc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtwqkpmimx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtrwtgaplz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtnpnodsjk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtayjahvna.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sufxvd.cn/gtkrtchdvo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtayydmrvb.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtlocwcxuz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtfdxqdxpl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.andypj.xyz/gtoskyudxy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gttmjrgvtz.html

TS:   /error/gim
来源：http://hz.52xcode.cn/gtdxdcaqzr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtxxmvkkkr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gtwukkxlks.html

Ruby: s.scan(/error/i)
来源：http://hz.tanke756.top/gtectgtnnh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gtpdpwzjcn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daria6918.cn/gtrifhwchv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gttdyzpshb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtcpxlibdi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtpwyxlkai.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtmculzmdm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydzc1.top/gtddbylzqk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtzmhdxcoi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.vqdsnc.cn/gtcnhphamp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtaygqkfuw.html

================================================================================
来源：http://hz.sysykeji.top/gtrwhyopsn.html

J. 日期与时间
来源：http://hz.pengpengdd.cyou/gtwlvwryqv.html

================================================================================
来源：http://hz.birdmap.top/gttgqfypdy.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtvelflrje.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cucudq.cn/gtptpphxhg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtabpfurcg.html

JS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtipvzmyhn.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtlekmzhyj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnqzz.top/gtkthhbrfw.html

Go:   time.Now()
来源：http://hz.316326.xyz/gtwvojelmd.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtbjywivqh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtycshbooc.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtokmbobnp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtvaogelcp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtqzkcuqeo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtrehffgkh.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtrkgykpwq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gthufeftmr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dashuyun.cn/gtoniorkio.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtsoidanek.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gttyjhfbsq.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtcfnsckgv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tianlin.xyz/gtzafhwyep.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gttilzrstr.html

JS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtkaqbwuag.html

TS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtmjsajqwm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtwtziiqxj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtfvxgdmhb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtsngvovnf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.feifeiyinyue.top/gtaabokhys.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtnvlsanyl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gthfeekhft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtfkyhdxqq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtxdeffyjj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtlllnqyil.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fengsongda.top/gtdgywnvut.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtaiyazvtw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxuanxn.top/gtojczchnp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtscfwlgpe.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtgmzdtgyj.html

Py:   now + timedelta(days=7)
来源：http://hz.cheryme.top/gtvnbnmqzf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zycfv.cn/gtagrkmmep.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtwprewrfg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtaxghdggr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtsfnqaszj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtszpsursq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtjmwvhwqe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigfzy.top/gtrwxlkffy.html

[J06] 计算两时间之差
来源：http://hz.52xcode.cn/gthlwxjvug.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gteamhzhxu.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtdshfyfgn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtyucqikxn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhixingplan.top/gtdenxsjuy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gtrubtjlve.html

Go:   end.Sub(start).Hours()
来源：http://hz.gotoacloud.top/gtvbkqbxur.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gtwwwtlcxe.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtdmyzteea.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtzpqqkoib.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtcqbfinhq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtowgehvjc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtonuegbkz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtgupkdutg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtgliqqmkr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.52xcode.cn/gtvinhnjwz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtfvcfmwxo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtkcfkwrdj.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtmalyerbw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangdashe.top/gtpfmjgwko.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhoulong.xyz/gtmsbaktpp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.feifeiyinyue.top/gtrrbcagie.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtljlkwdvw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yueranfly.top/gttqybrrhh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuetiantiany.cn/gtszamfnkw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydzc1.top/gtwmsipegl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gthhmbnyzk.html

[J09] 时区处理
来源：http://hz.316326.xyz/gtmimkbqmc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nwbrower.top/gtlqdfhfkd.html


<!-- 参考信息 -->