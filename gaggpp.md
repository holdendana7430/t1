代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.cdnleiting.top/gtyoxddgcu.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtdihkwztn.html

Java: public String getName() { return name; }
来源：http://hz.yonumen.top/gtbceeaeqh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gtcuepkxin.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtotsyadwo.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtvznckegc.html

[G12] 对象转字符串
来源：http://hz.vqdsnc.cn/gtojbghrnv.html

Py:   def __str__(self): return self.name
来源：http://hz.0kj1m.cn/gtuwruqftp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtldzjrmhy.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtabhysipi.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtcelelcpu.html

Java: @Override public String toString() { return name; }
来源：http://hz.havefunace.top/gtbvfcpifb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtvvqhwhre.html

Ruby: def to_s; @name; end
来源：http://hz.sxryk.cn/gttrsuguxb.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gthubvfevi.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gtvvppyzgp.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangtech.top/gtfnwfufdb.html

PHP:  $u instanceof User
来源：http://hz.yongpay.top/gtuskejxmv.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtmxwqyznl.html

TS:   u instanceof User
来源：http://hz.daria6918.cn/gtuicunajg.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtkpbyayre.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gtjahxigyo.html

Ruby: u.is_a?(User)
来源：http://hz.yueranfly.top/gtawzwlbim.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtsipdqxnj.html

[G14] 数据类 / record
来源：http://hz.shangyingyoupin.top/gtzhgqrosk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtiekbyilm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtxwbhjkuw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtmgcrficm.html

TS:   type User = { name: string; age: number };
来源：http://hz.haohaochexian.top/gtyzcdknsw.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtkcrazuum.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtvrcsgabn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtqjggqlyd.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gtnxckzomq.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtjmdgejby.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.havefunace.top/gtcjqqtjpi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258888.top/gtwvxhxvit.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtqvkghgja.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gttkvlmopj.html

Java: enum Color { RED, GREEN }
来源：http://hz.sweek.top/gtrztyzcbm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtqebqayiv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtxkbzchgz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtyrpspzpx.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtphiftoyo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xylfe.cn/gtfbpvfwhn.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258.top/gtltidzepd.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtzsakgxvm.html

TS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtvlvtkykr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgfzy.top/gthtrztrsr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gtmqtyqibq.html

Ruby: obj.instance_variables
来源：http://hz.quarkkingdee.top/gtwkxgpkif.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtvebczqjg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvvvkbjzr.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gtundkwjbl.html

================================================================================
来源：http://hz.ivvv.top/gtavkjzajy.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtxuaxtppi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jlsjyb.cn/gtkmmkxuhp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.c1oappe.top/gtgtjqviif.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtlecmcwfm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gtnyavvxyy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnxiangtu.top/gtselhitwv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtzsqimwel.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenlongwang.top/gtnaozhsed.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtdhzdzqro.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtvweqkfvw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tanke756.top/gttrxvsdkh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtickqrcap.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtdjapupww.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtcnvvulmx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtjjizgdsh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtpmbodqtm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gtkxsbmsiq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtovdioisd.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtlywmmili.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhiwuduotai.top/gtvwudllpr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtljkcvynh.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtftkanuwp.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtuneczjls.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtpbswbbyf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.kuanghao11.cn/gtfxqtfewy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gthfycrnhf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gthtiiugsf.html

[H04] 自定义异常类型
来源：http://hz.zhoulong.xyz/gtuqgpakqs.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtbvbxwqwx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtmsuhlmyv.html

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtiflrnjdj.html

TS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtuctfpite.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gttpdfurld.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtntpdeyll.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigfzy.top/gtjdewhvgj.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtdggdvjvr.html

[H05] 捕获特定类型
来源：http://hz.zhiwuduotai.top/gtbarrfauk.html

Py:   except ValueError as e:
来源：http://hz.zycfv.cn/gthwnpmqyn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ivvv.top/gtphcblmzj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtwkfocfos.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtcfjchobq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtxkuwkfjc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.9152youxi.cn/gtnndqvibt.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangtech.top/gtivbnleli.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinghuilouyu.cn/gtpuqszftj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydzc1.top/gtrdnuqnjy.html

Py:   value = d.get("k") or default
来源：http://hz.cashguo.top/gtebmrubmn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.vqdsnc.cn/gtieajvmxh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtizcdqxha.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtgtvdnfse.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gthxqsaoxy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gtjpbwcbka.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtscybccdb.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtbqdrghvn.html

[H07] 断言
来源：http://hz.fzhhl.top/gtztzkxukp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtqnizmlwz.html

PHP:  assert($x > 0);
来源：http://hz.nanxuanxn.top/gtrxomlzpa.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtcafusfck.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtgktriwle.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtnzdsgbya.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtkzxxplcc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.iojbl.cn/gtqdpwigkv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtpilhrwzj.html

[H08] 获取错误信息与堆栈
来源：http://hz.andypj.xyz/gtjzvutjmx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yonumen.top/gtdihvaezx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gthhwqdfjo.html

JS:   e.message;  e.stack
来源：http://hz.dianchejie.cn/gtmondsirv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gtrpbltzsz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtfytzyvvs.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtdsmvvapt.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtsjucdrro.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtbfloaain.html

[H09] 带错误码的异常
来源：http://hz.jqgfzy.top/gtniqtqxxo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sufxvd.cn/gtwplddbzn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtwakgbxxn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtogeohgix.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gtqzqliuwn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtbrduqsyf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gtxdsnywfh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gtervuufzm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtxsfrjjus.html

[H10] 资源自动释放
来源：http://hz.yj20258.top/gtcdrvqpqd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtburwwqhf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtfmzvdixx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtrjfyzyxe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtpvwaihaj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.meibo888.top/gtjbnxbksi.html

Go:   defer f.Close()
来源：http://hz.tianlin.xyz/gtouxbqmcb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenjidiqi.icu/gthpthlaxb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydjk.org.cn/gtaayluefk.html

================================================================================
来源：http://hz.52xcode.cn/gtmjaanlpg.html

I. 正则表达式
来源：http://hz.jinyuanbaomall.cn/gtgwhkskml.html

================================================================================
来源：http://hz.zhongyouzk.top/gtaizrkxvt.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtwmkndijr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtnptkatvq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtbkqdhorv.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtqleeiebr.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtccbisgnn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ppjwa.cn/gtlxxukpwg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gtmvvdwkyu.html

Ruby: s.match?(/\d+/)
来源：http://hz.xinyue.icu/gtkycmdkvj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydzc1.top/gtkguchwru.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtfggvhdhz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gaohongyu789.top/gthpfzxsae.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gtiusvgjpl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhaomingkeji.xyz/gtutsesgwv.html

TS:   s.match(/\d+/g)
来源：http://hz.ivvv.top/gtpzvqcaez.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydzc1.top/gtzwmakxig.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtdmlakybr.html

Ruby: s.scan(/\d+/)
来源：http://hz.aibaodan.cn/gtxsscanol.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtkjywojqq.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtthwniqou.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtsglnknmu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shzxlz.cn/gtktwvasxj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.feifeiyinyue.top/gtogaexltb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.mhx1999.top/gtkpuoflad.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtklarjfnc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangshuangyany.cn/gtemehzork.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtfidwbhfw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.snrcjt.cn/gtqfxszoma.html

[I04] 正则替换
来源：http://hz.nwbrower.top/gtyusgobvf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gthwfnjnwa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gttioeiwxr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtzgogdmfp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtxocborxj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuanzhike.top/gtidjigfzv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pycfn.com/gtitbutxjk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuanzhike.top/gtomrmiifw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hfpthk.cn/gthrhrrfhe.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtjpdyadik.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtopdralyn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtcqxazunk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtcjuhnzty.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gteemmiytd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.meibo888.top/gtzxdswxbw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gtkfhpckvd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtljhkmtsd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtxbhjrpxl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtkjmrbgja.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtpttklfbx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gtbxwcscas.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtcdqegvfz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtdhmkywkt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ydjk.org.cn/gtdluvdpdn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtmxrurdsd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gtckewahnw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtipqlikbd.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtfhlnemoc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zdqjudy.top/gtzkaxohyn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtydimsllb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtahkhcpuy.html

TS:   /error/gim
来源：http://hz.aibaodan.cn/gttsmmxrzg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtunhjvgfs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xylfe.cn/gtfgttcjdy.html

Ruby: s.scan(/error/i)
来源：http://hz.hnqzz.top/gtyeqjaeyh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gthyctgbks.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtwrvsdiit.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtjqyvjocf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtltthbrqw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtgbrdmthh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtwbotuutk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtyjmnkoeg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtntgakmal.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtnjmbmtfe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtifzadgja.html

================================================================================
来源：http://hz.jinqigufen.top/gtzqgrpilm.html

J. 日期与时间
来源：http://hz.nanxuanxn.top/gtdkuitmso.html

================================================================================
来源：http://hz.ivvv.top/gtniqtfpii.html

[J01] 获取当前时间
来源：http://hz.cdnleiting.top/gtvrzwpuwx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtwrxrerqg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtiteaspgj.html

JS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtsrdbdtzg.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtcmzjagfq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shangyingyoupin.top/gtjniqzroe.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gthhmhoaoz.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtnlwhuimr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guowangkeji.top/gtbmmkouod.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gtoosrsiwp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtdfufwajj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtlguckwsj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gthxslvayk.html

TS:   d.toISOString()
来源：http://hz.iojbl.cn/gtqbvtjkrw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daxiang520.top/gtdvjsbylj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtdnwkequi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtrdsuwpfu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xingfuxueyuan.xyz/gtjtvgllgu.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gtuuwtnpxk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gthjfhnegm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtnwdooekp.html

JS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtfswtyvbw.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtgmdzoprr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gthgayscbi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtpadwpykn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtgqlgrrub.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xinyue.icu/gtbgywogrj.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtxysxllte.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtmilcyuhw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtutvrvzym.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtxrheagfu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.svipenyu.cn/gtkdjuyilr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtizqhbrtb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gtknggxrun.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jlsjyb.cn/gttnhsezxs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtbhgrxgex.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtvevrcfwx.html

Py:   now + timedelta(days=7)
来源：http://hz.pengpengdd.cyou/gtwjvleebl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tanke756.top/gtrtsuuwgg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtmkhzlwvh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtovpgnzzh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ppjwa.cn/gtzirrpliu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xylfe.cn/gtvyjemyha.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtnslymnyp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sysykeji.top/gtnjtkhcec.html

[J06] 计算两时间之差
来源：http://hz.aizwys.cn/gtvtsrjhjy.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangtech.top/gtyplvaewl.html

PHP:  $end->diff($start)->days;
来源：http://hz.nwbrower.top/gtopkhzqqv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gtgvojkmoz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ppjwa.cn/gtszhdgvkp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtqgymnozl.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtqpgzneyk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtwqpysndo.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtnywnebhp.html

[J07] 比较两个日期
来源：http://hz.haohaochexian.top/gtohtqchow.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtnhlarubc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtwyxllxma.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtkxzcgumv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtmnwjweun.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtgovkicnm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gterfltdwh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtluhnsxan.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtqiuufcrf.html

[J08] 提取年月日与星期
来源：http://hz.haohaochexian.top/gtzfydpcfz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuxming.cn/gtggyvsqze.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxuanxn.top/gtgsfctsgs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtomcsdqii.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cheryme.top/gtrvxulxhh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gthcklfluk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtgphaxfog.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtlapcgrjo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuetiantiany.cn/gtavratkeu.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtowqsznop.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cheryme.top/gtdgwbdpul.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gtvsceqgfs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtevcjsvnv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtpyuodwqi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tianlin.xyz/gtnnjobxxo.html


<!-- 参考信息 -->