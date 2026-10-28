代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.jianghu66.top/gtolbboreo.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gthtnqaajx.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtgrsppszq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtuuopgecy.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtwwclavhl.html

TS:   get name(): string { return this._name; }
来源：http://hz.ivvv.top/gtvcpvkejz.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtpcqzkbru.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gtqosqxque.html

Ruby: attr_accessor :name
来源：http://hz.nanxuanxn.top/gtkjakkhdo.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtgzyplbvj.html

[G12] 对象转字符串
来源：http://hz.ivvv.top/gtymruhiuv.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtiyvpevqk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtyryqfdzg.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gtgxrfouph.html

TS:   toString(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtljiadegm.html

Java: @Override public String toString() { return name; }
来源：http://hz.0kj1m.cn/gteazhsood.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xylfe.cn/gtiljaoqta.html

Ruby: def to_s; @name; end
来源：http://hz.pycfn.com/gtkypkwftp.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtekqquslh.html

[G13] 判断对象类型
来源：http://hz.ehwqpu.com/gtqtixrcsc.html

Py:   isinstance(u, User)
来源：http://hz.daxiang520.top/gtnlydjexp.html

PHP:  $u instanceof User
来源：http://hz.quarkkingdee.top/gtzifdewoe.html

JS:   u instanceof User
来源：http://hz.yj20258888.top/gthzwhkdqh.html

TS:   u instanceof User
来源：http://hz.jqgfzy.top/gtzjcusosx.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtadkjlndz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtcdxolrvz.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gthyvkcmah.html

C#:   u is User
来源：http://hz.52xcode.cn/gtdthqfwec.html

[G14] 数据类 / record
来源：http://hz.tian-w.cn/gtkbamcoms.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtknmgpeqw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gogol.net.cn/gtjwulaibt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtusublxyv.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtwuafhfhf.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtgcofbgfp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daxiang520.top/gtjkcbsseg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zycfv.cn/gtfzulqynm.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gtfrmvubhw.html

[G15] 枚举
来源：http://hz.yuxming.cn/gtkytmoash.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtgazrlqlf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tanke756.top/gtbyedklxp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuanzhike.top/gtgljtajtx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtywdqyjau.html

Java: enum Color { RED, GREEN }
来源：http://hz.sysykeji.top/gtmlhcpljh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ybcxt.top/gtjixhvcoj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aibaodan.cn/gtvhotlvlp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtkoxadlem.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtaecozagz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258888.top/gtgefsoawc.html

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtlbbemkvo.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtanzqxngm.html

TS:   Object.entries(obj)
来源：http://hz.sweek.top/gtpzmymqzr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xinyue.icu/gtexnclssh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jianghu66.top/gtmowiqide.html

Ruby: obj.instance_variables
来源：http://hz.ivvv.top/gthutmvuls.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtxkfxngae.html

================================================================================
来源：http://hz.bjfxy.top/gtfwsphnbc.html

H. 异常与错误处理
来源：http://hz.hysaishi.cn/gtskdoprzk.html

================================================================================
来源：http://hz.ivvv.top/gtztyhqakk.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtsmyiebdc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gtridclsiv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sxryk.cn/gtacpmntli.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.svipenyu.cn/gtnvjscqkq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtfvziwvjo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ppjwa.cn/gtoaedvqmn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zycfv.cn/gtlsfdhrrg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnxiangtu.top/gtwkkzdxzs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nanxinkj.top/gtprttovwj.html

[H02] finally / ensure 收尾
来源：http://hz.yuanzhike.top/gtamwcifbs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ivvv.top/gttophyvcm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtncfukynm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtkvbkaokg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtrybgtgmw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gttuvcfcna.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gttsvvyrsl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daxiang520.top/gtgqfxzfws.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtgykxwteq.html

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtpbdvrvyw.html

Py:   raise ValueError("错误信息")
来源：http://hz.smart0.xyz/gtuykpqztw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtigbbzqfh.html

JS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtszwtkezf.html

TS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtrftqyvyc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtpwawmahc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.haohaochexian.top/gthjgdyimx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.bjfxy.top/gtrvoyyfzz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gteijsccou.html

[H04] 自定义异常类型
来源：http://hz.tian-w.cn/gtwmopxalk.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gtbdyqtqgz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aizwys.cn/gtvwjlzwul.html

JS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtucqypbtz.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtvjtfijzm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtbdwwbzod.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cqqwz.cn/gtzwvpbubs.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gtvegsrgrc.html

C#:   class MyException : Exception {}
来源：http://hz.meibo888.top/gtossglbjh.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtdbwkytam.html

Py:   except ValueError as e:
来源：http://hz.yonumen.top/gtobpnuupb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtamzwrdke.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gtvvgjtjzx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gtocwmvoro.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cashguo.top/gtvvtrifqa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtnthzumso.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtcboclkij.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.316326.xyz/gtgacaqset.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtnesmmasn.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtbcgvsflx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtprqrgkay.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtdeldewbi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtgcxsaarz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtutsfjbuv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhoulong.xyz/gtvyyfmfde.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ydjk.org.cn/gtavascuwh.html

C#:   obj?.A?.B ?? default
来源：http://hz.hysaishi.cn/gtmoebbzof.html

[H07] 断言
来源：http://hz.fzhhl.top/gtaramdbhe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtniqyudbn.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtysnlvola.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtdeemnqtp.html

TS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtwambjhaa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtqqotdxoi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gogol.net.cn/gtphgkyblw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtcfarslin.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtqhcrxhsz.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gtiawnrfhm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtobbttquh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhixingplan.top/gtjfxbopsv.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtrdvrkukf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zdqjudy.top/gtgtlgkkcm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtpqvjzesp.html

Go:   err.Error()
来源：http://hz.daria6918.cn/gtikwtxttb.html

Ruby: e.message;  e.backtrace
来源：http://hz.svipenyu.cn/gttkpkuqxd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cheryme.top/gtsxchidte.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtfqrambyw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtdkijxvoo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtuioqtohf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtbjihifak.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shzxlz.cn/gthyjzcnxn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtnrkhiasj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtuhbqwoap.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtnkklaiez.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gtkulgdrdg.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtepiuyldd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shzxlz.cn/gtelgozhrm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnqzz.top/gtnrriqsbw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtxprrurif.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gterprbmyc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtiyddymks.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtpguazjdy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtsadxlthu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtpcqpcnyk.html

================================================================================
来源：http://hz.daria6918.cn/gtweytrnoa.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtxuxebibk.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwfmnqubp.html

[I01] 判断是否匹配
来源：http://hz.yueranfly.top/gtondcfpwc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtdenbmlfc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gtowqepkjh.html

JS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gttvvtwume.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtdrgoizsj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cheryme.top/gtkexrhddr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtdipwuonl.html

Ruby: s.match?(/\d+/)
来源：http://hz.svipenyu.cn/gtjrkrcvyp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydzc1.top/gtnbnwfghp.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtlqxtittd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnqzz.top/gtksndeqpg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtjrimkqcq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aibaodan.cn/gthawbzcrj.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtcxzhezbq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtnwjblfqq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtxlpodqyn.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtqtlqkteo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtrdigglxi.html

[I03] 提取捕获分组
来源：http://hz.redwolf501.top/gtvtipzali.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtwmiinrpg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xylfe.cn/gtcursghah.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtjszsojix.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtdegguuqc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj202588.top/gtunubvkde.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sysykeji.top/gtyoyjkatu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtsmxjqjry.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ppjwa.cn/gthhyvhpvt.html

[I04] 正则替换
来源：http://hz.hongshengwenyu.top/gtozmywxsv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuetiantiany.cn/gtgcpcgmhv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtywciyupw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtgijkfsdu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gttjgmmcgc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtnrtcejnv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gthuwtojyk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gteuwkucfh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtvuwqsqsw.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtwsjobfrw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zdqjudy.top/gtvjlowrlo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guannengcc.top/gtjoathnli.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtgpohtrmj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtgfelzoqo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gttvejewwj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtvdysmkrp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtlffnpbkj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gtkuedigne.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtvkppoius.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtipfqdfln.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.bjfxy.top/gtjiffgqgl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gthnixplnf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtfxzigptz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gteoxhrrra.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtlevvpddm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtwpvrmvxd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtcnfwzyop.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gthhslfydt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtbzldgcoz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jiagoushi.top/gtwuphhqfr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtgqlyomal.html

TS:   /error/gim
来源：http://hz.hywenlv.cn/gtionllkor.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtdwdyvhrt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shangyingyoupin.top/gtjhtewbai.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gtbmvzukvd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xylfe.cn/gtudrkpmal.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangkeji.top/gteyehyhla.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtmzshsjxy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtdnuuemnc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtuiqfoath.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtmgddzold.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtnirmhxkv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tianlin.xyz/gtcgeuisrl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yangfankeji.com/gtwgokuhmx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gthxxnpbss.html

================================================================================
来源：http://hz.nanxinkj.top/gtwzibdwtk.html

J. 日期与时间
来源：http://hz.birdmap.top/gtcjacvllo.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthknmsavh.html

[J01] 获取当前时间
来源：http://hz.ivvv.top/gtmulipdkl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtvpmiwenw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtzjyfphtu.html

JS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtgwgojklv.html

TS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtcyqxtllx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtemcchnbr.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtpbougqjc.html

Ruby: Time.now
来源：http://hz.9152youxi.cn/gtfpoediif.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtofdonatx.html

[J02] 格式化输出
来源：http://hz.birdmap.top/gtylctymjt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtvwyuxsii.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtulefnhzm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtgmgbowpw.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtxwhulhvb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtkeurqdos.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gttszztqkb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtqtcxkakb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tianlin.xyz/gtxcymmlso.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gtbdpcbtgs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jianghu66.top/gtjemgsmof.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shangyingyoupin.top/gtqmhvoozy.html

JS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtpudodhhe.html

TS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtxinwapmg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtoexyllfj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dianchejie.cn/gtogycrayo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtgtmwnzwf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtucnhuarl.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gteebvsmxr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gtkcbugked.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtckmrbkwj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtgakbmhey.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.svipenyu.cn/gtrxsqkolw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtsbujnlfs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtpmsxybra.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gthliikscs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtivwkgvti.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnqzz.top/gthpyprdhd.html

Py:   now + timedelta(days=7)
来源：http://hz.gogol.net.cn/gtsnhoeucn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtbhicbjfh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtjlwdiuxj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtmmbsadsm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gttyjjmvtj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtfpsrrmiq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtdihrxpzg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinghuilouyu.cn/gtpogfctks.html

[J06] 计算两时间之差
来源：http://hz.bjfxy.top/gticeccbfp.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gttvdrzpyx.html

PHP:  $end->diff($start)->days;
来源：http://hz.svipenyu.cn/gtcdzhnnks.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtxnzhmeqm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtpytybccs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jyoumei.cn/gtjzreunad.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtkeczasxc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jlsjyb.cn/gtuajpztgv.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtbetzcrjf.html

[J07] 比较两个日期
来源：http://hz.aibaodan.cn/gtchatirrd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtuutzmfvy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shzxlz.cn/gtfuoazywl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtgipltvnh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtojxoqlqu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jlsjyb.cn/gttiumyfrs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.birdmap.top/gtylmzzeml.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtfwzchhbe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtdunppjyg.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtzytfedse.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.316326.xyz/gteyrhhvto.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtejwkxgay.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtuupipbzi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ybcxt.top/gtxgmkzxhx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtmynafbpk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jyoumei.cn/gtwrfsrixd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenlongwang.top/gtpjztbaqg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aibaodan.cn/gtjtnfytrb.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtagopuaaw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yonumen.top/gtdrheuedi.html


<!-- 参考信息 -->