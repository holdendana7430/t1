代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.cqqwz.cn/gtmvcxttiv.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtoyzntjqo.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gtqxewnjdf.html

Py:   def __str__(self): return self.name
来源：http://hz.zhoulong.xyz/gtqydphlje.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtpjfxdssx.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtbcmforwv.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gttxjontkl.html

Java: @Override public String toString() { return name; }
来源：http://hz.snrcjt.cn/gtirktibmp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtmzswjsbw.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtjljutadb.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtnmemzwvb.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtbeevfwga.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtgixbsvij.html

PHP:  $u instanceof User
来源：http://hz.ybcxt.top/gtyofebehq.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtaobkdybo.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gtzevsydbm.html

Java: u instanceof User
来源：http://hz.hnxiangtu.top/gtferxebym.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fengsongda.top/gtyaxkvoqx.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtgzttzwzm.html

C#:   u is User
来源：http://hz.hfpthk.cn/gtgxtykonu.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gttfbqhmxr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtwxnrhvyh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gteqahxllz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtabfhabyg.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtwtrjgbjr.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtkfryziqf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.snrcjt.cn/gtnghlpery.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydjk.org.cn/gtovttdftd.html

C#:   record User(string Name, int Age);
来源：http://hz.yongpay.top/gtiwkwspsx.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtcwhlvsor.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gtskrwqybq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dianchejie.cn/gtmjolbept.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.52xcode.cn/gtaipeewpy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtrfmywurx.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtamfxrhyz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenlongwang.top/gtqjpnrymc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gttpzgxcec.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtivmymjyk.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtwwjmiagi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.iojbl.cn/gtaphqakxp.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgufenzy.top/gtpkijmdih.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtoxhzjygc.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtggzxjsew.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtkdwcvmyw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yongpay.top/gtjbqkbsml.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtuypdgqyc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cheryme.top/gthuexyirk.html

================================================================================
来源：http://hz.shuidangran.top/gtcekggftx.html

H. 异常与错误处理
来源：http://hz.wangdashe.top/gtxtyckoqp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnzbleruh.html

[H01] try / catch 基础
来源：http://hz.snrcjt.cn/gtbpmvebhd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.kuanghao11.cn/gtdecorjes.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.havefunace.top/gtpudckwop.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtvtasjfgd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtdfqreacz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.mhx1999.top/gtlpnydztn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gtiwlbnjik.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnqzz.top/gtizorbzcs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ehwqpu.com/gtlqgqezyy.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtckjtnwqo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtjeocfzge.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtoxditiuy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtnebkctpj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtunjpaqmr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtzpvtknnt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gthwsrwcgu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtmpfgummb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gtqnuwksed.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtuffeujoz.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtgeotxdot.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtjjnxobgu.html

JS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtuzfzqbjl.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtvgvsgyzq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtcmdpkwsq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtazqvlyla.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtgdofljda.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtbxcuatpr.html

[H04] 自定义异常类型
来源：http://hz.c1oappe.top/gtxvppqnof.html

Py:   class MyError(Exception): pass
来源：http://hz.kuanghao11.cn/gtqwjsxbpa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtczojvtfk.html

JS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtsevgzeqa.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtqxkhbefz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtmxvqcmwy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtrtmrfumj.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gthxjquwqh.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtpgvrnckn.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtjywooska.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtqxfrmujo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daria6918.cn/gtyihnfkon.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtohqwfkmw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtdnpcnqqs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fengsongda.top/gtealappti.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangtech.top/gtbzcfvrkx.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtiggsiwqo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ivvv.top/gtdvhdnajf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtwqerycov.html

Py:   value = d.get("k") or default
来源：http://hz.snrcjt.cn/gtiboofpft.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gttrametlz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtqasmjqbk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtedvofgmv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuetiantiany.cn/gtxabrpzzw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtchuvcogs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgfzy.top/gthpaswngl.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtpnuafvrc.html

[H07] 断言
来源：http://hz.iojbl.cn/gtfdxphzyd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.snrcjt.cn/gtxvnojkhh.html

PHP:  assert($x > 0);
来源：http://hz.daxiang520.top/gtkjvebykx.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtqiwjaaew.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtggeejzpt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtrcdjpfup.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtcxbjshjd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtshsqrkeb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gtdnewjjdl.html

[H08] 获取错误信息与堆栈
来源：http://hz.smart0.xyz/gthqvvghyj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gtrcqxenpf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtowoalaaq.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtrwigeprn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtwidvcoec.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtfsntvdrd.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtafgvmbkx.html

Ruby: e.message;  e.backtrace
来源：http://hz.cheryme.top/gtidsnwehm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtohbvzjxl.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtficgxzeg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hongshengwenyu.top/gtagsdiqgj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtfqfhltux.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jlsjyb.cn/gtrhtuyuqm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtlsudzsin.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtedzuknty.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtzssfwien.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.pycfn.com/gtpvgjnmpk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cashguo.top/gtruxupozg.html

[H10] 资源自动释放
来源：http://hz.daxiang520.top/gtypesubrn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtgummxypi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhongyouzk.top/gtqxnrxnoz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gthngaxksn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtdvcbhtxz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gturbzbezu.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gthevfpqti.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gttqqzrejz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gtpludqiro.html

================================================================================
来源：http://hz.jqgufenzy.top/gtubbyzkgi.html

I. 正则表达式
来源：http://hz.chenlongwang.top/gtkydtqrmh.html

================================================================================
来源：http://hz.zdqjudy.top/gtrqqtufns.html

[I01] 判断是否匹配
来源：http://hz.zdqjudy.top/gtfshsucfs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhengqikj.top/gtkusfwjtf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtrctgppho.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtrvswenhi.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gthjookweu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fengsongda.top/gtqqaihmkq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.mhx1999.top/gtorbaqtnw.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gtcomlkgcp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenjidiqi.icu/gtebyfwege.html

[I02] 提取所有匹配
来源：http://hz.jinyuanbaomall.cn/gtmyuhyxgm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtogwnvawi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.meibo888.top/gtueidesyh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtxiytqecu.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtzrqjsmsu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtjpvrxlvg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yanxiufei.cn/gtomgrilrw.html

Ruby: s.scan(/\d+/)
来源：http://hz.sweek.top/gtwnnragex.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtrpkbuqqw.html

[I03] 提取捕获分组
来源：http://hz.zhijiandao.cn/gtpducwgdn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gtosaaujuk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.c1oappe.top/gtvgxdptqt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtnnfytntu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gtoaruxsmq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinghuilouyu.cn/gtmnwchsco.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtdtzcwwuz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtrambbmlk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtncizuyyw.html

[I04] 正则替换
来源：http://hz.yj202588.top/gtynmfpdtp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gthcxugrwh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtoynclykx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gthmznopbw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtowiegbrq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ywan-chungtsiang.top/gtykbdwxns.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangkeji.top/gtnavjezce.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shangyingyoupin.top/gtbnpyzome.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtcsdcitpo.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtvcercimo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtthnbtnku.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sweek.top/gtlrrgzlwf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtottufhpt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gteioijzll.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gtycnqfyzo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cashguo.top/gttoguojom.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gthpjehrrb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guannengcc.top/gtbexnqkgb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gttbieqjfk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtkgnblhty.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtnrkirjts.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtavcrlihm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtuopfagrx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnqzz.top/gtkwnwpfwn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gttkebcxca.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gtwxlhjvze.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtuestovwm.html

[I07] 忽略大小写与多行模式
来源：http://hz.hfpthk.cn/gthwymaasi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhengqikj.top/gtyccsqook.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jyoumei.cn/gtedmalmpg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gtlznhqwxw.html

TS:   /error/gim
来源：http://hz.havefunace.top/gtgvqzyblh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtksvxhmip.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxuanxn.top/gtiljlwlyr.html

Ruby: s.scan(/error/i)
来源：http://hz.jiagoushi.top/gtlaifrequ.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtqmvjzyli.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtsoytzxqv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gteoenbxvf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gthobhilhl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtnyftkcjz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtooyobwbr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtlkrirint.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hammf.cn/gtrfuyyaws.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtheddskax.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtgqachwmg.html

================================================================================
来源：http://hz.jyoumei.cn/gtddpkkrqb.html

J. 日期与时间
来源：http://hz.zhixingplan.top/gtswtorteo.html

================================================================================
来源：http://hz.pycfn.com/gtzcllkuyj.html

[J01] 获取当前时间
来源：http://hz.ydjk.org.cn/gtzycipavw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.meibo888.top/gthdffwbaj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gthnjqrmfh.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtriixjfot.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gteqrvbqwt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pengpengdd.cyou/gtevswuiww.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtareksgvk.html

Ruby: Time.now
来源：http://hz.yj20258888.top/gtnptlarty.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj202588.top/gtvnxljqkn.html

[J02] 格式化输出
来源：http://hz.jqgfzy.top/gtuyhuqyrb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtsgyeotnb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtftocfksa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtxetrpygg.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gtrjuskywl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xziqi.cn/gtoknmjxdm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhoulong.xyz/gtrsuyrvpu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtwqojyfwe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangtech.top/gtwdnopxrd.html

[J03] 字符串解析为日期
来源：http://hz.52xcode.cn/gttedehlcy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhiwuduotai.top/gtdhfllvhk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydjk.org.cn/gtxljwwmrw.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtaydwiwdj.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtrbwxdklv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gturyihdyd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cheryme.top/gtfqdhsmrm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtimsfoyhw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guannengcc.top/gtvxcclone.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gthcfviull.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtzphpntdp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj202588.top/gtwlfoyszy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtuqzeucts.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigufen.top/gtgyerevgm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gtzvcysnyd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuanzhike.top/gtpznndcmv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gtmyiioqch.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.birdmap.top/gteiibocid.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gthcafevlh.html

Py:   now + timedelta(days=7)
来源：http://hz.pycfn.com/gtsaqnbgwo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtfzxcglwb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtljnwqcsb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtgmuobhmx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gtxorehgmm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtfqdkuzyu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtevwbclkt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtjgdtrnwd.html

[J06] 计算两时间之差
来源：http://hz.andypj.xyz/gtzrrrqahn.html

Py:   (end - start).total_seconds()
来源：http://hz.jinyuanbaomall.cn/gtyophhxpr.html

PHP:  $end->diff($start)->days;
来源：http://hz.gaohongyu789.top/gtlqtgrgfd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hfpthk.cn/gtjzkepjbf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.smart0.xyz/gtfmgvqnwu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jiagoushi.top/gthlqowgfv.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtwoffetkt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yanxiufei.cn/gtpecvolfk.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtgwzpfdhl.html

[J07] 比较两个日期
来源：http://hz.sxryk.cn/gtijqhihol.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gttvhfiqyh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtkbqvgfay.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtmyycalst.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtjfssduor.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gthopkinkp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtoiiugqxj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtytpgctst.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtoydamqhr.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtbzlglrdo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtsxjtqhrb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtpajaemii.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cheryme.top/gttjylishf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tianlin.xyz/gtzfdqxocy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtzaxxenbj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtzshetnvi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtqrhuipyp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gtakcycxhw.html

[J09] 时区处理
来源：http://hz.xylfe.cn/gtyhhxontp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtcjtyydbb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtxirgnpos.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gttfioztbu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtvefoconm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gturwxtdce.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtjybemsoh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.quarkkingdee.top/gtslhylkra.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xinyue.icu/gtfevbasef.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtnbnmjkcb.html


<!-- 参考信息 -->