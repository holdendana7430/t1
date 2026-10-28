代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.haohaochexian.top/gtxgedlcsi.html

[G11] getter / setter
来源：http://hz.birdmap.top/gttivoktng.html

Py:   @property 与 @x.setter
来源：http://hz.jyoumei.cn/gtiilrmuuh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yongpay.top/gtqhfykznn.html

JS:   get name() { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtwsnrsawb.html

TS:   get name(): string { return this._name; }
来源：http://hz.vqdsnc.cn/gtgeatjslj.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtowjxujol.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnqzz.top/gtybqbtqoy.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gttrpoknki.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gtparppzah.html

[G12] 对象转字符串
来源：http://hz.iojbl.cn/gtcxzxnmxf.html

Py:   def __str__(self): return self.name
来源：http://hz.hnqzz.top/gtpnmveumq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtmvwbjvtg.html

JS:   toString() { return this.name; }
来源：http://hz.nwbrower.top/gtvnzldbhp.html

TS:   toString(): string { return this.name; }
来源：http://hz.tanke756.top/gtdcudahfo.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtoemvnzuc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258.top/gtednvbzmc.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtwwtjtejv.html

C#:   public override string ToString() => Name;
来源：http://hz.pengpengdd.cyou/gtdpigzpif.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtqdntfuvb.html

Py:   isinstance(u, User)
来源：http://hz.daxiang520.top/gtnogysikx.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtkkihldcw.html

JS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtwxnfrhhg.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtynldsmgo.html

Java: u instanceof User
来源：http://hz.yuanzhike.top/gtttnumqfw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhongyouzk.top/gtefaabwrm.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gttagrxtnm.html

C#:   u is User
来源：http://hz.yj20258.top/gtioyvlzte.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gttuebgcyc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtrqsjhksj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zdqjudy.top/gtghfiqhnp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtwsealdap.html

TS:   type User = { name: string; age: number };
来源：http://hz.hysaishi.cn/gttwogxeza.html

Java: record User(String name, int age) {}
来源：http://hz.tanke756.top/gtmbkpkizg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtnnfpcpby.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fzhhl.top/gtgifmxdbr.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtxiyqrtmc.html

[G15] 枚举
来源：http://hz.zhixingplan.top/gtpvxazinz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gtskplzmos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtmjlmyfhw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gtjlrlszpb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtnohcfkgm.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhaomingkeji.xyz/gtnetextor.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cheryme.top/gtrrzubblb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gtlmolymcu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtxtarjprw.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgfzy.top/gtbxcujdap.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gteqkxywgn.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtjmvxojka.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtjvzjvhhl.html

TS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtgyzdryhc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtrsjfsrgv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtbfougowf.html

Ruby: obj.instance_variables
来源：http://hz.birdmap.top/gthvxsthel.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtgpnxwbvl.html

================================================================================
来源：http://hz.cdnleiting.top/gtdtujxlyf.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtzwrueugi.html

================================================================================
来源：http://hz.jinqigufen.top/gtfmtqecmv.html

[H01] try / catch 基础
来源：http://hz.meibo888.top/gtmkujmban.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtjogdrkri.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtkyrzyses.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtysrstaba.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gtaycziuik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhaomingkeji.xyz/gtzpytgknh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxuanxn.top/gtokvergji.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gturwwktnb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtqhsmtupv.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtnjcxexbb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtudzqwpad.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtishptqcj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtjsqjkzyj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtaffcruvu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtxydbuwrs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gtyjkqjbpr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gtgcopxebn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.mhx1999.top/gtjbiwbira.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtmvilemlp.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtdlnegozc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtvobufjqm.html

JS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gttlqsvhzn.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtnmctnjls.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtntchswim.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xingfuxueyuan.xyz/gtdhaeygjf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pycfn.com/gtwmtaljhm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.birdmap.top/gtepmqkvcn.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtovearvnw.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtdzlibcqd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yongpay.top/gtfbupwgdy.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtsmhntzbr.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtufmwypvg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtbimxiuam.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gthrxzfuyy.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtqqlgobmx.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtnmgjxwbf.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtlvswdqxj.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtbufrjykr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.iojbl.cn/gtcozozdpz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtgrvavhte.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtvbzknkyh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gtxbdaxexs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gthitxbewk.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuanzx.com/gtixigqaac.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nanxinkj.top/gtmsnqdcbq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtcelveqpc.html

Py:   value = d.get("k") or default
来源：http://hz.jqgufenzy.top/gtxycqgtik.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj202588.top/gtvziknuvb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtxrawnvsc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtnecdercf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhixingplan.top/gtabcrcpsz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtgklnhviq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtrhcajegx.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtcfxhwlkq.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtdyotcppu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigufen.top/gtaeqaibbb.html

PHP:  assert($x > 0);
来源：http://hz.zhiwuduotai.top/gtwnhfmnjv.html

JS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtlrdagilr.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtctpynljm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangshuangyany.cn/gtszydjlhq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gtzmfewixc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fzhhl.top/gtzrsbhcvq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtkvobojor.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtqllxrgmi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtbugelhrj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtsfkcpmph.html

JS:   e.message;  e.stack
来源：http://hz.zhijiandao.cn/gtlxxohtht.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.meibo888.top/gtktzolwbq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtlcfmchag.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gtbbxdikfo.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gtlvnydxdc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ppjwa.cn/gtdirtndzc.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtyocpgync.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ywan-chungtsiang.top/gtlcinayfc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnxiangtu.top/gtwlgjeaho.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ywan-chungtsiang.top/gtmhpuhvgi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigfzy.top/gtjjlnixcp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gttsblvxvt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtkupxfvww.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.0kj1m.cn/gttjyspflr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtshmfsmpx.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gtqbelptvo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.havefunace.top/gtvnwweivf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtdhzktpix.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtoewxhyvu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtpwsoewub.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtgenofnyo.html

Go:   defer f.Close()
来源：http://hz.sxryk.cn/gtnyluidsy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtwsflytqj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuanzx.com/gtbeyudyfl.html

================================================================================
来源：http://hz.cdnleiting.top/gtzwgjiiia.html

I. 正则表达式
来源：http://hz.ydjk.org.cn/gtdhnnwrxq.html

================================================================================
来源：http://hz.tianlin.xyz/gtcwewkbtc.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gtyblcxqby.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxinkj.top/gtfeluxbix.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydjk.org.cn/gtfebxpjgt.html

JS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtiioddgvw.html

TS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtnnsshljm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cucudq.cn/gtnbdileeh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gthoasikyw.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtoqktucfz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtnchpmgmg.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtafhdbpzf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtpffsegww.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xinyue.icu/gtneynvrqa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtiaudamle.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtpadoerdx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gteshazmpe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yueranfly.top/gtjdcdoszp.html

Ruby: s.scan(/\d+/)
来源：http://hz.gotoacloud.top/gtovuggaha.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yonumen.top/gtsgpdazje.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gtcruhjbun.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtksfbeebp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gtajeqzhez.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigfzy.top/gtlkvcksux.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtzzwzfdql.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258.top/gtjhkmzptl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gtncvewooe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gthpkcsmxk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hfpthk.cn/gtbhitehel.html

[I04] 正则替换
来源：http://hz.yonumen.top/gtxdtxxyrc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtfkzamgxy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtyidjldtj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtsnsndwxo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtqdbxeeju.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gtscrrppzs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jianghu66.top/gttrgkbkpl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gturecwizo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gogol.net.cn/gtgaqurffj.html

[I05] 按正则拆分
来源：http://hz.guowangkeji.top/gtayaxvczc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtmrvnngec.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.316326.xyz/gtfgoposnf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtvbsbhqwi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtsfnoulzj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jiagoushi.top/gtuwgymulf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sxryk.cn/gthaavpbhn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtdpcjkqcv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtioxrxhnw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.redwolf501.top/gtybajquju.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtoypalhmt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtitflvmxh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtwhkthwhw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtvyyceasl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.havefunace.top/gttxfictnd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangkeji.top/gtkozfwgfm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gotoacloud.top/gtptttfhbj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtthhrjmmh.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxinkj.top/gtvdeajsyz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtblvvjrrv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigfzy.top/gtwlzbsjoj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guowangkeji.top/gtdelxydzc.html

TS:   /error/gim
来源：http://hz.yangfankeji.com/gtibhgebga.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtnxfgeets.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtbyyxxzex.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtjmkpsdcn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtbtvlsfvb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtsspqovks.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtntzkbqld.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ehwqpu.com/gtebpxpvaj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtleblcqls.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtrvamckwq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtgcqydvuy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sweek.top/gtqpndoqeo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtjmnllzop.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtmfosuogu.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpkbxxefb.html

J. 日期与时间
来源：http://hz.zhaomingkeji.xyz/gtldfwshzy.html

================================================================================
来源：http://hz.jqgfzy.top/gtgbujntuu.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangkeji.top/gteiqfqvhg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangshuangyany.cn/gtozxzbvjw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtbekxnffg.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtibhhlcet.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtlazvyjxj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ehwqpu.com/gtzqwdhvvo.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtkifakryv.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtmnoptbzy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtxrdrhvpd.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtmipytotc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtaalweknw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtxvcwsgww.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cqqwz.cn/gtniwtrwqr.html

TS:   d.toISOString()
来源：http://hz.feifeiyinyue.top/gtflezuyqq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cucudq.cn/gtijcnmjcc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.vqdsnc.cn/gtighfhnsp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtrjrqazxj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yonumen.top/gtebhahvbh.html

[J03] 字符串解析为日期
来源：http://hz.sxryk.cn/gttpzmsody.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtnzzuqlhg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yvedp.cn/gtkxerjpsy.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtobcbofvb.html

TS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtzzrbtjls.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtvbvdhtmc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gtnttflggb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtehytmwcf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gtbiqkrqyf.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gtqkskgarr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtyayaxzrz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtybxscluv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtqaqjaruc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangshuangyany.cn/gtshsueauz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydjk.org.cn/gtpwtmghse.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gttofhlyyr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gtisjafrnj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xylfe.cn/gtatcmdgyz.html

[J05] 时间加减（加 7 天）
来源：http://hz.cheryme.top/gtqaqrumjd.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gtzeshdrqp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtylyhkfvn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gttlnmzwta.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtiasdhphy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtktldzmid.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtxxurhdaq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtdtqksmft.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtzpffubhk.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtbyhgtmes.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigufen.top/gtuygcsggw.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydzc1.top/gtvxlnyqud.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gttpicwqvr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.9152youxi.cn/gttuxlscgb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gttkbnznsk.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtgdzrgiyh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtbbwstdlh.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuanzhike.top/gtcmaydbcg.html

[J07] 比较两个日期
来源：http://hz.zhaomingkeji.xyz/gtknvzavdo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtuftmflvg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtlelirvzo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtphbiwjfj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtxlowsdnf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtsevbzxln.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuetiantiany.cn/gtgosumaak.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtzqytcatx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtabheztkq.html

[J08] 提取年月日与星期
来源：http://hz.hywenlv.cn/gtctzgrbbg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gttiasknay.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtirprusez.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtgwjggnck.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.snrcjt.cn/gtfgrytlnz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xziqi.cn/gtzqaysjzt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtgxnafhjb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dianchejie.cn/gtgnpfnowr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258.top/gttxlkkddd.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtwerodwev.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtqfoepjzs.html


<!-- 参考信息 -->