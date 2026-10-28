代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.xylfe.cn/gtxakgvidd.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gthzvtzlld.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtobkepxwx.html

Py:   def __str__(self): return self.name
来源：http://hz.aizwys.cn/gtocwqjhcf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtuhyeinlp.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gtaqejsifl.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtzmhtjyqv.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtudxpnwja.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtcbhqpzgq.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtvlcrkedl.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtrdeynecf.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtgetwbuws.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtoclybhke.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtcictuahg.html

JS:   u instanceof User
来源：http://hz.hywenlv.cn/gtvegevooh.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtalnwhdgx.html

Java: u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtslocozsh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtqjvyswmm.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtckgbohme.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtqbcgmhpn.html

[G14] 数据类 / record
来源：http://hz.xingfuxueyuan.xyz/gtlmvxqhfm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtxspyidyw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ppjwa.cn/gtrcbpbxhs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cashguo.top/gtbmzeiyut.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtzkvxiies.html

Java: record User(String name, int age) {}
来源：http://hz.kuanghao11.cn/gtjeripplk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.smart0.xyz/gtoofjkfxv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gtcoihglkv.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtvfhjraol.html

[G15] 枚举
来源：http://hz.birdmap.top/gtejnlsyyz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.iojbl.cn/gtfnefqlfo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gtmoypyklv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuxming.cn/gtpmzkxcov.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtnjihxalt.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtlgwftxsj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hywenlv.cn/gtexifjsja.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtunmybrhj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtivtacanw.html

[G16] 对象转数组 / 字典
来源：http://hz.chenjidiqi.icu/gtwfxqeepk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtpijrjaop.html

PHP:  get_object_vars($obj);
来源：http://hz.zhongyouzk.top/gtevnednqi.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtidexljpn.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtsqfoihof.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.bjfxy.top/gtqnhaehiz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtkswfiifb.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtlnawjuoc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangshuangyany.cn/gtjgtjkbnk.html

================================================================================
来源：http://hz.shuidangran.top/gtspwkkeyy.html

H. 异常与错误处理
来源：http://hz.sufxvd.cn/gtzkfmnzul.html

================================================================================
来源：http://hz.nwbrower.top/gtokuzsygr.html

[H01] try / catch 基础
来源：http://hz.snrcjt.cn/gtfszbtjpx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj20258.top/gtqeeexkmq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtydslrvqy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtpmkscysp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.bjfxy.top/gtdhwyzjar.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhixingplan.top/gtgvndmjgu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtnluaixsg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.meibo888.top/gtncmegmny.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangtech.top/gtyefojtnk.html

[H02] finally / ensure 收尾
来源：http://hz.zhijiandao.cn/gtoirnjiuy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtzcymczui.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtyxcvhbom.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtrtmrocrm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtphpavgkj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gthytqapcg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtgpfofebs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtngngmkmy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhengqikj.top/gtbixuhzoe.html

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtixpxqfkk.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gtboblfosb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtlhkgnmdx.html

JS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtxdcrvfql.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gttpxzapjt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtfhflhegv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuanzx.com/gtqerteclk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtxkttynhp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gttmxgptru.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gtbymqhiwv.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtidobcmgq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtkyeqcqht.html

JS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtvwnkpuqd.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gteuibedkl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtahorvcqr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhaomingkeji.xyz/gtpnrjynhk.html

Ruby: class MyError < StandardError; end
来源：http://hz.sweek.top/gtnayqmeec.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtvysynhwg.html

[H05] 捕获特定类型
来源：http://hz.cqqwz.cn/gtaucbpqcd.html

Py:   except ValueError as e:
来源：http://hz.gaohongyu789.top/gtbceqimbr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtpqfpilol.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtqbxriank.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtqenihgsy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtehxtazlz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gtphekyiuf.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gterraavyz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gttjuushbr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gttyapqidg.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gtsnieixha.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtkmmdmcyh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtwmbigpsq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtxexvtjgu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtiahsguae.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.haohaochexian.top/gtqvvarcbb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtmmgtxjao.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtlnwjvtbw.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtegwximii.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtvrgtahtq.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtjvlbrqlo.html

JS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtpexqitwz.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtprywwwag.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ywan-chungtsiang.top/gthzvqidph.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtrhvntodc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtpwvnoylm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.kuanghao11.cn/gtqsxgzrli.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuanzx.com/gtqaqbkxrs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fzhhl.top/gtklcymhdk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtynjzbbys.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtvletyurk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtfewmfuvj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtpwosceas.html

Go:   err.Error()
来源：http://hz.daxiang520.top/gtimfomypi.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtnfschfeg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jlsjyb.cn/gtgkogpndj.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtqbqtbbqt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtiixmzmua.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gtddgogici.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtuwwqzkxm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shangyingyoupin.top/gtprflczas.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnxiangtu.top/gtbyszooym.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtgnbfohna.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigfzy.top/gtcxmxefyz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtharktldg.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gtskoldpuw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhongyouzk.top/gtomrlpwrd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinghuilouyu.cn/gtdcemsgtn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtvncaxefz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtokjuguhr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtubvribjd.html

Go:   defer f.Close()
来源：http://hz.nanxinkj.top/gtkdfzjjca.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shzxlz.cn/gtxbsakcfn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yongpay.top/gtyiatizhb.html

================================================================================
来源：http://hz.snrcjt.cn/gtwlkfsgyb.html

I. 正则表达式
来源：http://hz.yj202588.top/gtqjqwgdfj.html

================================================================================
来源：http://hz.snrcjt.cn/gtuqufyhyw.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtryjtilsj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtnmybdpuk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtyujvqdrg.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtnydkdgie.html

TS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtzzeerfyv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.meibo888.top/gtuloqhazm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yanxiufei.cn/gtjtbpafer.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenjidiqi.icu/gtfemqxggw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtaxqheoqq.html

[I02] 提取所有匹配
来源：http://hz.9152youxi.cn/gtctgqbqnx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtygoufbtb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gttkyuhlix.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtzidevsjz.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtmdvuwmuh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.meibo888.top/gtefwtmgal.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cheryme.top/gtfbwtcsgp.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtsgbysabr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgufenzy.top/gtbrvpwysk.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtqrnfgaky.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtozyleium.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dianchejie.cn/gtdooqfhky.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuxming.cn/gtooncnwzm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.aizwys.cn/gtmaoavigj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gteeaugmrx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yongpay.top/gtqxiohaet.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nwbrower.top/gtgqqdopjd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtrepuyrri.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtcjcjcfxm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.smart0.xyz/gtpnpftihe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtgtfqlsxu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtpnoyzmpb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtmlwixblw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gtqgkodtcq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnqzz.top/gtblkanmvx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtmvzsiypf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gtphtoixhl.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtyciwfwpo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xziqi.cn/gtostahocf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.smart0.xyz/gtbkgmzkpo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtcwdceybb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtfajwqrqb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.vqdsnc.cn/gtvpoibhzi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtjppiffgx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtjsygzhpm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydzc1.top/gtteymbikk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj202588.top/gtvnfwctgt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gthpdmdlld.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shangyingyoupin.top/gtbqajjizd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtmucarcpc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtkmezhcsv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nwbrower.top/gtdboebetw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gtustqutax.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhengqikj.top/gtioxnskyu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtwrnyzwbf.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtijhacahk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangdashe.top/gtjubocazj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gthtieslsn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtubccbftc.html

TS:   /error/gim
来源：http://hz.dashuyun.cn/gtlcmlytjf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangtech.top/gtlgzcaimn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gtfwjifctk.html

Ruby: s.scan(/error/i)
来源：http://hz.hongshengwenyu.top/gthemjxlwj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtbiraciml.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhiwuduotai.top/gtyizpuxiy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenjidiqi.icu/gtljhukgbf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtxzkmmxll.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtwzzgvysg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtajnwtmyd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtgeqpyoko.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gthgblbpvi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.vqdsnc.cn/gtubdljvrt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtridfpkhh.html

================================================================================
来源：http://hz.gotoacloud.top/gtssxeurzx.html

J. 日期与时间
来源：http://hz.quarkkingdee.top/gtjidedntm.html

================================================================================
来源：http://hz.yonumen.top/gtdrmxnlio.html

[J01] 获取当前时间
来源：http://hz.zhaomingkeji.xyz/gtetjopjwk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtmpaviytv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtnmoyxohh.html

JS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtilozvkfl.html

TS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtlwipvfmh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daria6918.cn/gtbmkziecb.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gtpduamwju.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtkhxvtlcx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.snrcjt.cn/gtngjmuqga.html

[J02] 格式化输出
来源：http://hz.snrcjt.cn/gtblutozgk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.mhx1999.top/gtuqqwljxd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtwwubhwxv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtbkppppma.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtsiqgxeem.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtlkwvyaqf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.9152youxi.cn/gtnhplszhg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtnuelerfw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ywan-chungtsiang.top/gtixidygyr.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtgqrquokg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydjk.org.cn/gtkncqngcd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jlsjyb.cn/gtsjuefnfu.html

JS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtjvpkkdjy.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtcjjddmnd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtmxowbsdm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gturehfepx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtsnljzxfo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtmlhcizog.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258.top/gtfmizghsm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtluyyebbs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgfzy.top/gtxdlahrhi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.iojbl.cn/gtrafsorca.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtlekiyyaf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gtteicwpjf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtcnefiszi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtiyedudws.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gttwlkydhi.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gthftenbka.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtbynnzmyj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.9152youxi.cn/gttxkirobx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtbsdmfwwd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtruztlyuu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtqrljjiot.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zycfv.cn/gteapdudes.html

Ruby: Time.now + 7 * 86400
来源：http://hz.havefunace.top/gtvjsdehvn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtglbbyvij.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gtdbzrkfib.html

Py:   (end - start).total_seconds()
来源：http://hz.pengpengdd.cyou/gthutymmmg.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtlabzpzmj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cqqwz.cn/gtuokssgae.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtkigwczei.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.52xcode.cn/gtsszxhexm.html

Go:   end.Sub(start).Hours()
来源：http://hz.zdqjudy.top/gtcbsxaovs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gtnvyywvvd.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtgaerbvqq.html

[J07] 比较两个日期
来源：http://hz.shuidangran.top/gthniknusi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gthvnitise.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cdnleiting.top/gtbpsdgtth.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtppgsooor.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtaglwnjrl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtrexlatav.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtxzatmjgk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtfbynydqm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtwhamqmwy.html

[J08] 提取年月日与星期
来源：http://hz.zhijiandao.cn/gtcwuwvmyd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtymfnnpap.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtakondcsr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gaohongyu789.top/gtbsbhhvak.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xingfuxueyuan.xyz/gtvnkirwhr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuetiantiany.cn/gtonttybre.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.vqdsnc.cn/gtbjtxxdwh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gogol.net.cn/gtkaiikgmj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ybcxt.top/gtuukduddz.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtjdhnpskv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aibaodan.cn/gtsvowpnes.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gtsdqfrkws.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtpnogpsyz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtkvreurnq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtsuikrexe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtfjoeeoim.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtjgnfparz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtrlruwfvw.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtgidapgep.html


<!-- 参考信息 -->