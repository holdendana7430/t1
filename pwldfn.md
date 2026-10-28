代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtesihboaq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ybcxt.top/gtnfgdttvo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtcrcrlfkz.html

C#:   interface IShape { double Area(); }
来源：http://hz.ybcxt.top/gtwgrzctdy.html

[G10] 访问控制
来源：http://hz.nwbrower.top/gtqsofhfcs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtkqhfpwie.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtwaqgmooj.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtbuxsblfl.html

TS:   public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtnupfnrcm.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgufenzy.top/gtkbpaffov.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gotoacloud.top/gtzujvflmp.html

Ruby: public / protected / private
来源：http://hz.sysykeji.top/gtqhoyegxa.html

C#:   public / protected / private / internal
来源：http://hz.9152youxi.cn/gtfyeuhjmf.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtklgoshri.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtxzhdfibm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtkqytxpgz.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gturkibhag.html

TS:   get name(): string { return this._name; }
来源：http://hz.c1oappe.top/gtvyxbxmhu.html

Java: public String getName() { return name; }
来源：http://hz.snrcjt.cn/gtjdyqsalr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daxiang520.top/gtajyfzfam.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtokthxskh.html

C#:   public string Name { get; set; }
来源：http://hz.ivvv.top/gthrexfmpa.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtlywrmhiu.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gtfpwnxtzu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtheqtazfi.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtzpuhufsf.html

TS:   toString(): string { return this.name; }
来源：http://hz.sweek.top/gtpipkvpko.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtcrfkuksj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtyxazoych.html

Ruby: def to_s; @name; end
来源：http://hz.yanxiufei.cn/gtxdifcaxu.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtgcfazqti.html

[G13] 判断对象类型
来源：http://hz.hnxiangtu.top/gthnyfgkde.html

Py:   isinstance(u, User)
来源：http://hz.jianghu66.top/gtwxsjqqje.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtylaftpzb.html

JS:   u instanceof User
来源：http://hz.c1oappe.top/gtvauofxsu.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtukqxjmub.html

Java: u instanceof User
来源：http://hz.daria6918.cn/gtchuarshs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.vqdsnc.cn/gteougqqat.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtllpvqfsk.html

C#:   u is User
来源：http://hz.hnxiangtu.top/gtnlluvcqw.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtjyvmecvu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtzcesigdn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.svipenyu.cn/gtpgkjygbr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.andypj.xyz/gtykfexmgb.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtvvwyhycm.html

Java: record User(String name, int age) {}
来源：http://hz.aibaodan.cn/gtzsajgxxb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fzhhl.top/gtnokenkby.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtdrlnyjis.html

C#:   record User(string Name, int Age);
来源：http://hz.xylfe.cn/gtkyofgert.html

[G15] 枚举
来源：http://hz.hnxiangtu.top/gtyuvieddx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenjidiqi.icu/gtcgrvyldx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtgyaxntjn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pycfn.com/gtyllacrit.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtrfhzusua.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydjk.org.cn/gtflrhiygn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gthsimetrf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtzqsalfqs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtyaxccqch.html

[G16] 对象转数组 / 字典
来源：http://hz.smart0.xyz/gthrwdbtbs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gthspyntdk.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtkzxodxyi.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtwzuibuhq.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtfgmtplqy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.snrcjt.cn/gtuxazabxs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tian-w.cn/gtukvznzgq.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtroaueuhm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.quarkkingdee.top/gtnionalvb.html

================================================================================
来源：http://hz.gogol.net.cn/gtwdccdofq.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtrgnminbf.html

================================================================================
来源：http://hz.hywenlv.cn/gtwbygsuup.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gtvkbdjima.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtmxirxzjj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtmdnqteki.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtlirbjoxq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtiixkbnpg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtdofokmzi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gttaftuchw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtcgafwwok.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinghuilouyu.cn/gtjwghygus.html

[H02] finally / ensure 收尾
来源：http://hz.zhengqikj.top/gtoodjmwof.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shuidangran.top/gtjzzscmja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtypkvlxvh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtwjnafswl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtmmkrgmip.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtqjrjfrkd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgfzy.top/gtvegcpoti.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtsbesghjm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gttimblmdx.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtsvnuovqq.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtfynqbvii.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtvpghbxwt.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtyivlkvpw.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtmqpkcaxn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtmlovmzuw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtqihhzamc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtfosmnjdl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtxguhyqzx.html

[H04] 自定义异常类型
来源：http://hz.tian-w.cn/gtpeuyoufz.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtsjfanonm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtevikqbjk.html

JS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtenagddfe.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtavxfrckx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtiecuqtxb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigfzy.top/gtsejvazmy.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigfzy.top/gtqpwenjvq.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtaawgnzrq.html

[H05] 捕获特定类型
来源：http://hz.cucudq.cn/gtusinopjd.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtdwubffxj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtvcbbmhvs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gttljzjpzy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtlsiwybge.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtzerjrwhj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xinyue.icu/gtyuxbrfcy.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtancjljku.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtrbojnxnv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yonumen.top/gtvyyimtok.html

Py:   value = d.get("k") or default
来源：http://hz.zhixingplan.top/gtbiegwthi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtyneedmws.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtpitqbych.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtpupenaha.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.52xcode.cn/gtlutwapka.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gtqselhnuv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tian-w.cn/gtcaosbujl.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtnrjdahdu.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtqkpabrcl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtrtmzckaq.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtkbobahzh.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtfkjnoowx.html

TS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtsdwaqhsx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gaohongyu789.top/gtnbszdspa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.birdmap.top/gtoobalzhv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xylfe.cn/gtdpqfltag.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtahgpxyrv.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtrciufvvf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gaohongyu789.top/gtmbcmskxd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.smart0.xyz/gtmgcaejrq.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gttyjgflku.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.quarkkingdee.top/gtdbxypjid.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tianlin.xyz/gtzoukoifb.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gtujrwtjbs.html

Ruby: e.message;  e.backtrace
来源：http://hz.9152youxi.cn/gtoyeqxioq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.iojbl.cn/gtanixypvp.html

[H09] 带错误码的异常
来源：http://hz.cucudq.cn/gtanvwmzsp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtmnjaldvl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gtxomuhjee.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gtqlmogwlh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gtwbxeksvl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gtuomcozmr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtndqcajkc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtrocsokcq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fzhhl.top/gtvfehjiss.html

[H10] 资源自动释放
来源：http://hz.chenjidiqi.icu/gtkopmooto.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtbnrswbbl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zdqjudy.top/gtxooiclik.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtflyahzmv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtvvxaxryh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.316326.xyz/gtmirqrsps.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gtrsezmcjc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtkxpsfpvh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gtgbhebisk.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmflwcpmd.html

I. 正则表达式
来源：http://hz.chenjidiqi.icu/gtrlleoyeq.html

================================================================================
来源：http://hz.316326.xyz/gtnjhywxxk.html

[I01] 判断是否匹配
来源：http://hz.c1oappe.top/gtsuqssvrs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtrrkgmssu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtendgiasi.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtaomznlvs.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtcdxvdrcu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtnkwwdter.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.kuanghao11.cn/gtnhqljdjy.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtuqbblbhq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hywenlv.cn/gtgacvztdd.html

[I02] 提取所有匹配
来源：http://hz.jinqigufen.top/gtrfjjyafo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtgwxjejkj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtbhotvmrf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dashuyun.cn/gtdaxiiiil.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gtfsixjlie.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.52xcode.cn/gtlnlvkrzy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtxjkyoegt.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtawrsxymx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sweek.top/gtrfszmale.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtzfulfzep.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtodenqkqr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.vqdsnc.cn/gtvdtvrult.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.snrcjt.cn/gtkxdrchlk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cucudq.cn/gtrdeoplqo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenjidiqi.icu/gtvvimiovb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shangyingyoupin.top/gtuctctzcq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxinkj.top/gtanzmqnxc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuanzx.com/gtdztfhlnk.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtohosswwo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jiagoushi.top/gtqdhdjxwv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtnknujlhs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtxmmrklrl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtohixfqlf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtetjwpvwn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gzhubu.top/gtmnelsyed.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtqjtmvwst.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtgyjgzxhe.html

[I05] 按正则拆分
来源：http://hz.ehwqpu.com/gtbexcbvpn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydzc1.top/gtkeblhlvv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhaomingkeji.xyz/gtbvrwksna.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtgspgaysj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtxkcuprih.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhaomingkeji.xyz/gtltofvbra.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtojzjtlbv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtwprlfcum.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtdukoinzb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinyuanbaomall.cn/gtghmauebv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtrdyautuz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinyuanbaomall.cn/gtqmdezfaf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtwuaygjay.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gteoyqphtc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cashguo.top/gthuiqlsuh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258.top/gtncychyen.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtwblkixqv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtjakqayha.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtuphitimf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtlhrleotg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtsffvadfe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gttlvbgdvm.html

TS:   /error/gim
来源：http://hz.hnxiangtu.top/gttqfcsupv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtnomkitmg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.svipenyu.cn/gthcjhndrc.html

Ruby: s.scan(/error/i)
来源：http://hz.xingfuxueyuan.xyz/gtjbnzfgkl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zdqjudy.top/gtmwsbjmub.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ppjwa.cn/gtuylnckts.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtezjystfb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cheryme.top/gtapcdegxb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtdzhfsixy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtlckzlrwc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtsurmtdoq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtpbuxlsyk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yvedp.cn/gtrhlicvcq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gthykswsdv.html

================================================================================
来源：http://hz.wangdashe.top/gtajgkimmx.html

J. 日期与时间
来源：http://hz.daria6918.cn/gtaehsbixu.html

================================================================================
来源：http://hz.nwbrower.top/gtrcuhkpyu.html

[J01] 获取当前时间
来源：http://hz.xuetiantiany.cn/gtduqfwoer.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtypemikwg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtjpwnpqhu.html

JS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtfhsjzhrn.html

TS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtbxsmmabw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtfgtizzsm.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtrnfunsqq.html

Ruby: Time.now
来源：http://hz.chenjidiqi.icu/gtbqfywjzx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtwedrrxda.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtazoujbmh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtihdjdhms.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtmltxstkq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cdnleiting.top/gtzweqsspf.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtisxhfhll.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.havefunace.top/gtdkxcwgtl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hywenlv.cn/gtehpskpzm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtuifvleiv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtancnxptl.html

[J03] 字符串解析为日期
来源：http://hz.gogol.net.cn/gtfcroogjs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258888.top/gtqoklcrqc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxinkj.top/gtqannrisl.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtobmccrba.html

TS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtpbuwkgyz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gttzttxqsw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gtyfqrlppi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtgfmrrtzi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gtatlvdugg.html

[J04] 时间戳与日期互转
来源：http://hz.xylfe.cn/gthrzgfbar.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fzhhl.top/gtrnaemsab.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtepjkppcc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.birdmap.top/gtojjfkpav.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xylfe.cn/gtlpcvqhvu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gtnoidwnyn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtcebglusf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtnynetvqg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zdqjudy.top/gtbwgpeczz.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtzgezusns.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtbpnxaqmb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtldqfalpd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtsxatynsa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtuxaimjah.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gthjvpqmwa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tian-w.cn/gtipivyjud.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cucudq.cn/gtwtvmaomi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gtpiiglyuo.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtfmezuqxe.html

Py:   (end - start).total_seconds()
来源：http://hz.smart0.xyz/gtcqboqdsj.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtodlqsuet.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sweek.top/gtusfwjtfb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtngrqazib.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtenidgtvb.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtazsuupan.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gtdbcqbgnb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yangfankeji.com/gtbmcgcxjt.html

[J07] 比较两个日期
来源：http://hz.xuanzx.com/gtncfbuvux.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtgbqzlsdr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtmqznckbm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtvojyavxi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtyvhoqadz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtnzgilbmh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gtdpdqwlqo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtxdkjsnqi.html


<!-- 参考信息 -->