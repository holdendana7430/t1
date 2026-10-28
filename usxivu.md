代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gthldplmvu.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gttpjdbdrn.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtxkzcwxym.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtxakuosin.html

JS:   get name() { return this._name; }
来源：http://hz.birdmap.top/gtloucmglh.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gturjooirc.html

Java: public String getName() { return name; }
来源：http://hz.cheryme.top/gtwamqumxx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtumqspmfo.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gtrmcmcxbl.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtfpjpuyuc.html

[G12] 对象转字符串
来源：http://hz.chenlongwang.top/gtyrskkvbz.html

Py:   def __str__(self): return self.name
来源：http://hz.sysykeji.top/gtqmkbruts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtjnprtzsd.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gttbfflksw.html

TS:   toString(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtkdsazptn.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtmldserhs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.havefunace.top/gtnzilobqx.html

Ruby: def to_s; @name; end
来源：http://hz.xuetiantiany.cn/gtyyjnlamo.html

C#:   public override string ToString() => Name;
来源：http://hz.sysykeji.top/gtsvjrgtcz.html

[G13] 判断对象类型
来源：http://hz.pengpengdd.cyou/gtgdcqsnvg.html

Py:   isinstance(u, User)
来源：http://hz.zhengqikj.top/gtstfodnrs.html

PHP:  $u instanceof User
来源：http://hz.haohaochexian.top/gtqimfajde.html

JS:   u instanceof User
来源：http://hz.ivvv.top/gtsyooqvqo.html

TS:   u instanceof User
来源：http://hz.sweek.top/gtuflkdsar.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtzedkahju.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtnxcjbjxr.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtmzvloklo.html

C#:   u is User
来源：http://hz.zycfv.cn/gtaspggxyf.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gtsdrkhfsn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shangyingyoupin.top/gtlwlrkedy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.quarkkingdee.top/gtdfhmqxsa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtiwmcbjkr.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtloojphxy.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangkeji.top/gtgrgahqvj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yonumen.top/gtrhnggxtd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gtkkudoecm.html

C#:   record User(string Name, int Age);
来源：http://hz.havefunace.top/gtywpvbajh.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtiymburbp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gtsqiugwaw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtvzqdqtez.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtsinxbgeb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtbsqhjjur.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtuaamwogu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtxleuymkt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtfznirafe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtsnawrxlw.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtgmcxsnxy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gthlpghamc.html

PHP:  get_object_vars($obj);
来源：http://hz.zhongyouzk.top/gtrzzmwaap.html

JS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtqmyruqrf.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gthqmduwdn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gtbqrpvhhv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhijiandao.cn/gtpyccbyvn.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtsvqudovz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gttqjwketf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtiprgvqeu.html

H. 异常与错误处理
来源：http://hz.sysykeji.top/gtcsnergwk.html

================================================================================
来源：http://hz.0kj1m.cn/gtehpvgmoy.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gttctrnjpx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtnxeccwlx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtbqohkwvu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtdnmsmwoo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ppjwa.cn/gtytmhgfux.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tian-w.cn/gtagxwunqq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtauysqxyn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtrmdekyms.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gtujpjrpyw.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtyjvqwkdh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guowangkeji.top/gtuirmldjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtiujyumvf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtpsxmplnu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtyvuqqygw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtmixykapz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shzxlz.cn/gtkgynrijl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtshlxxiaz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.birdmap.top/gtngegnhhz.html

[H03] 主动抛出异常
来源：http://hz.316326.xyz/gtpgehofuy.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtequbjoem.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtizykdnae.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtrrelciff.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtklmzgaxg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtaqjtrswe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtfhjqewjl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.snrcjt.cn/gtrpzhoscd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.birdmap.top/gtnwuzpqvv.html

[H04] 自定义异常类型
来源：http://hz.yj20258888.top/gtahmnqxzn.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtcagxhleo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtngrlekbj.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtxtdssvkb.html

TS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtdhnfdbep.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuxming.cn/gtnpxiccax.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtnlmtlkhw.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtiggfzqqv.html

C#:   class MyException : Exception {}
来源：http://hz.yonumen.top/gtrxjprsyd.html

[H05] 捕获特定类型
来源：http://hz.hongshengwenyu.top/gtnbrlaueo.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtnyrnbjcu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tianlin.xyz/gtrijhuvnt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtqqptuuef.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtzgzebtxz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenjidiqi.icu/gtfutbmlwf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gtmyhotbxy.html

Ruby: rescue ArgumentError => e
来源：http://hz.meibo888.top/gtzodwdzjl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj202588.top/gtkyxuzpxh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtxqaeflyd.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtghxmgitz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtauxccjdm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gttobkapur.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtmoxfuvif.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtzubcqaqb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gtcndbsjaz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtejapciru.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtkhcfxlfy.html

[H07] 断言
来源：http://hz.yuxming.cn/gtcezuthiq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtdjsrzecv.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtbdvftzsr.html

JS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtryrcxnln.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtzznxlaoc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gtkebcaacj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtqnpmznpc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtveuferbw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtnsikqril.html

[H08] 获取错误信息与堆栈
来源：http://hz.tianlin.xyz/gtjgfvrqma.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtohapzrqk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj202588.top/gtfovkxdcx.html

JS:   e.message;  e.stack
来源：http://hz.chenjidiqi.icu/gtqaukikwr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.snrcjt.cn/gtwtqqozjg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtmsiepuxa.html

Go:   err.Error()
来源：http://hz.ybcxt.top/gtlmkejwai.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtvpraoqkv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtxumgrdau.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtmkufqojw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.mhx1999.top/gtyinlhpxb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sysykeji.top/gtovznmbka.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtbkppyvvb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxinkj.top/gtiggqfxpo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gtjtjiphpe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtmywksqmv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtytgqdppa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtjnphvijf.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtpwfsksfw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xylfe.cn/gtpsuhbaxl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xylfe.cn/gtxgjtdqpj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtbbyjvari.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtvafbjsrr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gotoacloud.top/gtdrzkfeuq.html

Go:   defer f.Close()
来源：http://hz.fengsongda.top/gtulynebcu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dianchejie.cn/gteshenqvq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtbahujnhn.html

================================================================================
来源：http://hz.0kj1m.cn/gtungpubvu.html

I. 正则表达式
来源：http://hz.shangyingyoupin.top/gtvicqmoxh.html

================================================================================
来源：http://hz.bjfxy.top/gtsyxdooca.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gtvfcfhdgg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj202588.top/gtrumzqtyw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fzhhl.top/gtnbbutxcy.html

JS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtjdhcmkny.html

TS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtbvfkcsre.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtvnctoiav.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gteziorgic.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydzc1.top/gtmrlxubem.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gtszqxdrol.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtgowttmyh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shzxlz.cn/gtnghekjsb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtdhhglexd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daxiang520.top/gtfngumequ.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gtxdgdclmk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xinyue.icu/gtjniqajyv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gtoegqfqqw.html

Ruby: s.scan(/\d+/)
来源：http://hz.shzxlz.cn/gtmhfbhkbx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yangfankeji.com/gtuduskzmh.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gtqmjqfhjr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtmokehnnv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guannengcc.top/gthushbpfe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtrxwpfilk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtixnjklna.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtaekokhfc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.52xcode.cn/gthgltltzc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hongshengwenyu.top/gtcesuydsb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtkoexjahp.html

[I04] 正则替换
来源：http://hz.yj202588.top/gtprtazxai.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangtech.top/gtvezzoxvh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtdjlngjih.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtxlxiqbcy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtfawfscyv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gtwhpjfraq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtbkmsrxrg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtyvipgdcn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gtyfahzflf.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtiboxaziq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhongyouzk.top/gtrqacpnkw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtcmwlktnq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtkigrrlyv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtpxzijwmn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cqqwz.cn/gtqiyaunve.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258.top/gtdepwjvsz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtazlevdxr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtxjbiqwuw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtwafatxui.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtjktbcvnx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtkxujbgys.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtobwfdhug.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtseetnzkb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtekaxkmrn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtdhosyodd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtjdaeoaku.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtctvrinlf.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenlongwang.top/gtimfpmevi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtsdzrhcfm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.9152youxi.cn/gtuigzijlf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.birdmap.top/gtuyicczxf.html

TS:   /error/gim
来源：http://hz.ppjwa.cn/gtqanjxnkb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtpklfugcj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnxiangtu.top/gtgarpxgjw.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtluowggqw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.kuanghao11.cn/gtbbljdnkr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtuarrwlci.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ehwqpu.com/gtbqkycsrj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtfpgezjgj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gtnvqldnyq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtxyyllead.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gtkalnnvsv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.mhx1999.top/gtkawgvfsm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.vqdsnc.cn/gthvshdilg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtcadmrpqd.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtovodvbha.html

J. 日期与时间
来源：http://hz.cucudq.cn/gtzoucwfut.html

================================================================================
来源：http://hz.tian-w.cn/gtdbngvdmo.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtievsjpnx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtxjxuajtt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtvzbzcahw.html

JS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtilzvpuis.html

TS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtcvuciztu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtmvgghlrp.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtenfgraxo.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtwlzidpqa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.haohaochexian.top/gtpkfyjqll.html

[J02] 格式化输出
来源：http://hz.jyoumei.cn/gthuichuel.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtokqoigap.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtaztjigir.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guannengcc.top/gtumsolvnf.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtcplujbst.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtyhakbhmx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtsftkipbf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtcxcyetal.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daxiang520.top/gtfdeacebr.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtpjycdyvg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtdomqhgxs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ppjwa.cn/gtasisivdn.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtzmuyxnxi.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtidegmcgz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtsxhdfwdr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gtzxprshye.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtgcmabhjt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtflvlmapi.html

[J04] 时间戳与日期互转
来源：http://hz.vqdsnc.cn/gtsoyhynbk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.52xcode.cn/gtkhjajneb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cdnleiting.top/gtwbxsfmhx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtmanhksyd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtcgrkiiwx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinyuanbaomall.cn/gtiyfmcflm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gzhubu.top/gtknkjvssp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.mhx1999.top/gtydmxyawn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtecfxynym.html

[J05] 时间加减（加 7 天）
来源：http://hz.havefunace.top/gtdxisjirr.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtziaqwnws.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.havefunace.top/gtpnocjjzg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtzcjyjmud.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtpbsrjmhi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtheuoezlz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtjcfkpigl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tianlin.xyz/gtpxzrfzzz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aibaodan.cn/gtrjuzznoz.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gthlaklswy.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtfkpqofor.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtzaiocavf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gtxnpddfgm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtkzvpnpxg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtwfztlqtl.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtnovziwdr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhoulong.xyz/gtrccemqgg.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gtjkaqgfev.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtfqgfuxwe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gteaysgfnf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gotoacloud.top/gtlrxlxfjq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtbzfdegmg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtncjelexf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gthkblmmqv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shangyingyoupin.top/gthxvjfrjg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtyzoelpxo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtzocwddqt.html

[J08] 提取年月日与星期
来源：http://hz.iojbl.cn/gtxrepdjvf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guannengcc.top/gtrahbyfuw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtwyirqwwq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhongyouzk.top/gthwzkurpm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtrhzbmqdx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtwinesgmn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yvedp.cn/gtarentbiy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jlsjyb.cn/gtfcqqniik.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhixingplan.top/gthorgjxlv.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtenwadluv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gteydmfuqu.html


<!-- 参考信息 -->