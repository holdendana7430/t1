代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.chenzaomai.com/gtpihesnee.html

C#:   public string Name { get; set; }
来源：http://hz.jinyuanbaomall.cn/gtzobeutwd.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtzjwnixkw.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtrsfwrcfr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtvbkpvpqv.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gttgabwple.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtsfhjkqka.html

Java: @Override public String toString() { return name; }
来源：http://hz.daria6918.cn/gtbqjyzsup.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtubevnkoj.html

Ruby: def to_s; @name; end
来源：http://hz.zhoulong.xyz/gtjlwxtgwz.html

C#:   public override string ToString() => Name;
来源：http://hz.guannengcc.top/gtoxuvwbhx.html

[G13] 判断对象类型
来源：http://hz.haohaochexian.top/gthqhhotdo.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtzmoedlsf.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtwulfdlso.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtjouerfvy.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtbrcqbqhr.html

Java: u instanceof User
来源：http://hz.ivvv.top/gtkisjjtho.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gtmbuobhqx.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtfugnxtbh.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtqwsuotvg.html

[G14] 数据类 / record
来源：http://hz.hammf.cn/gtewsyzpds.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.birdmap.top/gtyucnkwfo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtgmvwywab.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtdjorakpu.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtvylqrxde.html

Java: record User(String name, int age) {}
来源：http://hz.feifeiyinyue.top/gthurndhyw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtjjoneqzm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxinkj.top/gtqhiruiuu.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtiagatani.html

[G15] 枚举
来源：http://hz.52xcode.cn/gtuteelxuf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtgtvrvgdf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnxiangtu.top/gtfdacluay.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtnpwteofj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtavmyoumd.html

Java: enum Color { RED, GREEN }
来源：http://hz.vqdsnc.cn/gtxfxxfkxe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtjfndupuy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtwzwjswwl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtauspbuol.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258.top/gtydvfhnny.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.iojbl.cn/gtcbnzpwxc.html

PHP:  get_object_vars($obj);
来源：http://hz.yangfankeji.com/gtmzdbieet.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gthrygletb.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtztodptlt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtazdnomox.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtklmwqxrr.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtmecclqzx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gogol.net.cn/gtksnjokzu.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtlfmwdhuc.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtsephkazv.html

================================================================================
来源：http://hz.shzxlz.cn/gtivxpdipj.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtbnemjnwg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gtogqtwbcf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtbinyxdnl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtyvexkiku.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pycfn.com/gtdznbjjta.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nwbrower.top/gttekbzqla.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zycfv.cn/gtervtedtt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtglpxarrx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuanzx.com/gtdtcpypsd.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258.top/gtnairziqj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gttvfrzgqi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtkqkihuoq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtumfhyiuo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtjelvocje.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtkvfkfvka.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gttooyxoql.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtgyjrsccy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.mhx1999.top/gtmhdigmax.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtdaniuuzx.html

Py:   raise ValueError("错误信息")
来源：http://hz.yangfankeji.com/gtzuccferd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtbfxdeltz.html

JS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtsnakhtef.html

TS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtrxoooozs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtrouwubaz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guowangkeji.top/gtxhojttug.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtjkawpadw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtbeuakaae.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtfosulqln.html

Py:   class MyError(Exception): pass
来源：http://hz.feifeiyinyue.top/gtswqxpkqy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtbonoxcde.html

JS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtblgdajak.html

TS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtocgibiyl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sweek.top/gtfsenmsiy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yanxiufei.cn/gtasthzqom.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtpdwmhjnn.html

C#:   class MyException : Exception {}
来源：http://hz.hammf.cn/gtmpaawlgz.html

[H05] 捕获特定类型
来源：http://hz.yanxiufei.cn/gtdwzylufr.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gtygwngfga.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sufxvd.cn/gthqpowqxz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtlqweidaq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtxknfnomu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gtxhrdiili.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guannengcc.top/gtjvjypywa.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtgpfvnioc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yueranfly.top/gtjagtmgql.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hammf.cn/gtilcuazmg.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtebwuchtp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtcnzfbhdr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtddoaxxgq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtmvcyfuhf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtktfwbzld.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.quarkkingdee.top/gtshdexorj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.316326.xyz/gtwfxcqivx.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtwcsymqvx.html

[H07] 断言
来源：http://hz.birdmap.top/gtilxtprbb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtqvkrezkb.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtdlkszggi.html

JS:   console.assert(x > 0);
来源：http://hz.haohaochexian.top/gtawsdibbd.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtnldlrkkn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhaomingkeji.xyz/gthnsjqzte.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fzhhl.top/gtmezmwojz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtosdcqmmj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtzdooqvmq.html

[H08] 获取错误信息与堆栈
来源：http://hz.shzxlz.cn/gtvlhjfgrf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtsogtlicn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daria6918.cn/gtosgzwqsf.html

JS:   e.message;  e.stack
来源：http://hz.c1oappe.top/gtpwuvtgxc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhijiandao.cn/gtzvicdvyd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtgeppyxof.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtulwdoefy.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtfejarkhr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtoqkkyfvk.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gtkfrfdsdo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gtwcloqtlz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenzaomai.com/gtfscuaaqq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pycfn.com/gtmduthafq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hammf.cn/gtjzusfpax.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtqmnuhdkm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtbrdogdrk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtrolcljih.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cqqwz.cn/gtpvqcarvf.html

[H10] 资源自动释放
来源：http://hz.iojbl.cn/gtieytsfwa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtojstiabh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtcqmlefwn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtkxugxnnj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtgfibpqjk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtqqmaoggd.html

Go:   defer f.Close()
来源：http://hz.sysykeji.top/gtsabuneep.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtcrvedfeu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xylfe.cn/gtuaizxpcv.html

================================================================================
来源：http://hz.cucudq.cn/gtftxyeqrh.html

I. 正则表达式
来源：http://hz.zhongyouzk.top/gtidkdhtkf.html

================================================================================
来源：http://hz.jianghu66.top/gtluqpgtlr.html

[I01] 判断是否匹配
来源：http://hz.yj202588.top/gtfqbxjtyl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtbahbwkkt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtnffmmqsl.html

JS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtmjzxqamz.html

TS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtwipsoqjd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtypgxchye.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zycfv.cn/gtcjvafkcu.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gtjpcabdtw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.quarkkingdee.top/gtibkpjskq.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtfyxzgaru.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtnrzhqbay.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtrzyujmwp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gogol.net.cn/gtlakesjic.html

TS:   s.match(/\d+/g)
来源：http://hz.guannengcc.top/gtuviqsxlz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtbmafibut.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangshuangyany.cn/gtztupoife.html

Ruby: s.scan(/\d+/)
来源：http://hz.daxiang520.top/gtbvudisno.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtamswtghm.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtapmvfofc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.havefunace.top/gtdmedsrwk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtyibqdbsn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.52xcode.cn/gtscfodzhf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gogol.net.cn/gtecjcyfce.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtgjtlznhd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtewrzljyh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtlpdfveqj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtsnmnllny.html

[I04] 正则替换
来源：http://hz.meibo888.top/gthwueqqip.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtqsyngocs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtujaupruo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtvxqqnudf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ybcxt.top/gtoestlxqa.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtjicjxpkx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gtxrhqneew.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtozqdoakl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hongshengwenyu.top/gthcnrtfhi.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtldesltwt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtujwhcnco.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtvrwdjptm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtzvamwipw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtpvypnivh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yueranfly.top/gthzklxsqz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ybcxt.top/gttxueiqgf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtrduiojkp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinghuilouyu.cn/gtrxclrtox.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtjgylgtzn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtskqwlqoj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxinkj.top/gtrhshjitk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtllgdmrog.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtrqzliyoy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.bjfxy.top/gtpwxkmsqw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtwuhsaawq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtptzvyxnx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtwschtqac.html

[I07] 忽略大小写与多行模式
来源：http://hz.fengsongda.top/gtznqoqnoe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.andypj.xyz/gtagwjcisc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gtmcyimxub.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gtealbkkfk.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtzqjdjxyt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtlrvdfvte.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zdqjudy.top/gtdahgcxeo.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtnyzjumgy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtshucnbzp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangtech.top/gtxuraqlsk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hammf.cn/gtwbigvytu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shangyingyoupin.top/gtxalnbuzj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtumdwzyms.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtdzkblxfh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gthsolghbr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtadpxlnek.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtblzdomzu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pycfn.com/gtnqebnppw.html

================================================================================
来源：http://hz.yj20258888.top/gthzkbqvpc.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gtleyijdhl.html

================================================================================
来源：http://hz.birdmap.top/gtvtmhdyqu.html

[J01] 获取当前时间
来源：http://hz.yuxming.cn/gtuaatvvmh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtabnhfhyk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtukrgtjlb.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtneqjncdp.html

TS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gtemcfxmap.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangtech.top/gtuuqppxwn.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gttidaacwn.html

Ruby: Time.now
来源：http://hz.zhengqikj.top/gtkvrvjqwz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.snrcjt.cn/gttbofolsn.html

[J02] 格式化输出
来源：http://hz.xuetiantiany.cn/gtulvrdree.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtyrfmldyk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtzslisxgs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtvccaffdd.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtnhqvucaf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fzhhl.top/gtqdrwbnbe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dashuyun.cn/gtbxujbinb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtagwekvpu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangshuangyany.cn/gtofshejql.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtbwiyjwno.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ehwqpu.com/gtbugltbgn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.svipenyu.cn/gtspkfuhcf.html

JS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtaxgunzqw.html

TS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtnbpnbrfn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtxyxjdsgk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhoulong.xyz/gtrctclcqf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtpdfjxbah.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258.top/gtuljsxmmb.html

[J04] 时间戳与日期互转
来源：http://hz.feifeiyinyue.top/gtgetuzdpz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtzflmfajf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangshuangyany.cn/gtqkjjsmer.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtoedoaxqp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtxmcyqrzv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtejiumkxc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtmprsnzzz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tian-w.cn/gtneqdxiws.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtfkxpfxqo.html

[J05] 时间加减（加 7 天）
来源：http://hz.gaohongyu789.top/gtigddpegj.html

Py:   now + timedelta(days=7)
来源：http://hz.xuetiantiany.cn/gttmudbduu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuxming.cn/gtxcxiiqwx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtysfzxrft.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtyqldkfrd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtuaydafdi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sufxvd.cn/gtbyouuece.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtikagcond.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtvclbvady.html

[J06] 计算两时间之差
来源：http://hz.bjfxy.top/gthmoufmov.html

Py:   (end - start).total_seconds()
来源：http://hz.yanxiufei.cn/gtaslfxwkb.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtkrmzygin.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtxikmcnrn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydzc1.top/gtpicqzrkv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtfgiboklf.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtpljqidkg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jianghu66.top/gtzrmmwemm.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtaahjfvzt.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtzrhsszta.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtplgtvcft.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gtgrhmleww.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtkgakpbqa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtjtszofpv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtudtkerct.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jlsjyb.cn/gtwghhzhov.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtyvxrquvo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtnahgwvfx.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtazqsklmx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtiwwhldlj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydzc1.top/gtqamgorlj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gtxbkhtiqq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtckhndzem.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxuanxn.top/gtagyqphcs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtfajomtxj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhixingplan.top/gtxsnyakho.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtmxhbdknl.html

[J09] 时区处理
来源：http://hz.zhixingplan.top/gttklpxypt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtxxmmtvza.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258.top/gtdscvbela.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtqyeiqmet.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtxrtkwpgy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guannengcc.top/gtmtniibjv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.c1oappe.top/gtpiywxuqw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.andypj.xyz/gtfwigmhtj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gtjdzzraaa.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtduopdnqu.html


<!-- 参考信息 -->