代发 wailian999

[G10] 访问控制
来源：http://hz.gzhubu.top/gtviemetpq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shzxlz.cn/gtpxuxrrfi.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtdalfyxwb.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtzvzbhsux.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtuvvrypxd.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gtovpjqgvn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtueiegmzf.html

Ruby: public / protected / private
来源：http://hz.xziqi.cn/gtcrzmwzqg.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gtecympepo.html

[G11] getter / setter
来源：http://hz.shangyingyoupin.top/gtfdkavblw.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258888.top/gtcsewpetc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtuudqlvid.html

JS:   get name() { return this._name; }
来源：http://hz.yuanzhike.top/gtkuznyfom.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtysiayrci.html

Java: public String getName() { return name; }
来源：http://hz.zdqjudy.top/gtwkppasaf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtewotdsch.html

Ruby: attr_accessor :name
来源：http://hz.jinqigfzy.top/gtgaqumryu.html

C#:   public string Name { get; set; }
来源：http://hz.ybcxt.top/gtdxwdpjem.html

[G12] 对象转字符串
来源：http://hz.fzhhl.top/gtyrxxlnzj.html

Py:   def __str__(self): return self.name
来源：http://hz.birdmap.top/gtfronjjqd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtrujaplqv.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gtxfvqvhkj.html

TS:   toString(): string { return this.name; }
来源：http://hz.fengsongda.top/gtotfzenfb.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgfzy.top/gtmblzydll.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ybcxt.top/gtzxnohvlt.html

Ruby: def to_s; @name; end
来源：http://hz.sufxvd.cn/gtwbrmapyi.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtyxmdrywz.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtkqebayki.html

Py:   isinstance(u, User)
来源：http://hz.cucudq.cn/gtlvkdcdpc.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gtprtyasad.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtstsxhfws.html

TS:   u instanceof User
来源：http://hz.xziqi.cn/gttqfiqkuv.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gtyqehsliw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.meibo888.top/gtoigawbvh.html

Ruby: u.is_a?(User)
来源：http://hz.jqgfzy.top/gtxnvllhen.html

C#:   u is User
来源：http://hz.gzhubu.top/gtdvsvkhii.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gttwumrzbh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtdiwfoufo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtgnxbdcyh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtescwrzqc.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydzc1.top/gtvfgkilyx.html

Java: record User(String name, int age) {}
来源：http://hz.aibaodan.cn/gtgbtvsndb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtxtllfejo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtwgqxiifj.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtbadbbfoq.html

[G15] 枚举
来源：http://hz.yueranfly.top/gtzxvmimuu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydzc1.top/gtooxcxjxs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.vqdsnc.cn/gtbqfylsah.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gttxpelbmt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtvrtstwfe.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gttfsctjgo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gtgplahncr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shuidangran.top/gtfnmdzrla.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtwkadrlrx.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtnzqitday.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sxryk.cn/gtqftvhfow.html

PHP:  get_object_vars($obj);
来源：http://hz.pycfn.com/gtjxmevafk.html

JS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtnqwgapwn.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtqlpwkpqm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtnffnsgbe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtebsukami.html

Ruby: obj.instance_variables
来源：http://hz.aizwys.cn/gtqdymnbma.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtscyohuju.html

================================================================================
来源：http://hz.havefunace.top/gtqwbiggub.html

H. 异常与错误处理
来源：http://hz.shuidangran.top/gtpzdclfzi.html

================================================================================
来源：http://hz.hysaishi.cn/gtsgphppom.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtzvfwsuwt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gtclnzffjn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtrqtbzypt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtcnyeirjn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtbqvdwzth.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj202588.top/gtkjqwxlgq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gthdqtmnbm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydzc1.top/gtebanrjmc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtbwwvfdnm.html

[H02] finally / ensure 收尾
来源：http://hz.nwbrower.top/gtwwoalelr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gtbyckcnag.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtsjeoipjx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtjddjrbeq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtzqvhebui.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtwzzbojkx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gaohongyu789.top/gtwiowzlyn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtecaghkfl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.0kj1m.cn/gtqkwyqaqs.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gticuayjla.html

Py:   raise ValueError("错误信息")
来源：http://hz.yvedp.cn/gtkojnpwjv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtwmfadjvy.html

JS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtpcwbxlxf.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtlouietba.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gthgrlzwyr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xziqi.cn/gtopsdexex.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtoigytjwr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtvufqqjog.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtivqxalkn.html

Py:   class MyError(Exception): pass
来源：http://hz.jiagoushi.top/gtpzpkdahi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zycfv.cn/gtzgiyvibn.html

JS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gterkfldqu.html

TS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtdqaibowo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtdzxongsb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtdmuudurn.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gtrjlrrwng.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtzslaogbb.html

[H05] 捕获特定类型
来源：http://hz.smart0.xyz/gtpqvuhsyb.html

Py:   except ValueError as e:
来源：http://hz.gzhubu.top/gtqkupxxop.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cdnleiting.top/gtlyjjkixr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtjkrsedde.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtztdbihsg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.mhx1999.top/gtryidoumh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gteutyqyxv.html

Ruby: rescue ArgumentError => e
来源：http://hz.tanke756.top/gtoimqgbaz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.andypj.xyz/gtilxvczyb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.bjfxy.top/gtzltqwers.html

Py:   value = d.get("k") or default
来源：http://hz.zhixingplan.top/gtneznwcnr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgufenzy.top/gtkwbjvezy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtgusubnzl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtfqrapijq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.andypj.xyz/gtjnbwpfss.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhengqikj.top/gtfwuwwlug.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtscbkdcet.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtlbawayww.html

[H07] 断言
来源：http://hz.gotoacloud.top/gtyvhcjhaz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtgkfzvaxs.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtvsfmvymh.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtarcjitrs.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtkgstgttv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtgjnupifz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gogol.net.cn/gtzsqeceyg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtohrncijx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gogol.net.cn/gtkoipinyb.html

[H08] 获取错误信息与堆栈
来源：http://hz.c1oappe.top/gtxuibuibc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gtqmvozndx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gtwdnzgwva.html

JS:   e.message;  e.stack
来源：http://hz.yuanzhike.top/gtpndfdubk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258.top/gtgdmolcfi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtufyvxsft.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtojkneaxn.html

Ruby: e.message;  e.backtrace
来源：http://hz.smart0.xyz/gtfqtjmeps.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydjk.org.cn/gtibevcwwb.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtlmcxcssb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gtfxebkuxr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtgcceaqbs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xinyue.icu/gtmbjnubys.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtruaejlci.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yangfankeji.com/gtijngdnny.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sweek.top/gtafmvliif.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigfzy.top/gtsofvcwii.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtyeddnvgs.html

[H10] 资源自动释放
来源：http://hz.yonumen.top/gtzfzxjqqc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daria6918.cn/gtjreqhfom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gticvzekdj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtondwihaw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gterpfekih.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangtech.top/gtgwynxtfs.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtjdwrehjm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtjqhucirn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.kuanghao11.cn/gtzvaibela.html

================================================================================
来源：http://hz.yanxiufei.cn/gtusxqgdcx.html

I. 正则表达式
来源：http://hz.jinqigufen.top/gthguyyuio.html

================================================================================
来源：http://hz.cashguo.top/gtqtwuzrff.html

[I01] 判断是否匹配
来源：http://hz.hysaishi.cn/gtcgwbcfqf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtzyozbetq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydjk.org.cn/gtscpcbdjt.html

JS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtkuguqmih.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtywrpqurc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtmueazevi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhengqikj.top/gtsuchnceu.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtljmxtfzx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtxqpzrqwp.html

[I02] 提取所有匹配
来源：http://hz.shangyingyoupin.top/gtqoabqiti.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtwptnjwrp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jianghu66.top/gtivvkktig.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtkygfzgfi.html

TS:   s.match(/\d+/g)
来源：http://hz.sxryk.cn/gtsbxjiwws.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtlhbnolhl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtzsladnjs.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtiwmdvhjz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tian-w.cn/gtnbrobbrb.html

[I03] 提取捕获分组
来源：http://hz.zhengqikj.top/gtygrqpuwj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtvaxkhebl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gtikrxdbxb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gttwetmfcb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gtyawkhkox.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtbsehgpaq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtsecfqacv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yvedp.cn/gtddyipjod.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gtkwavyvwl.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtwocqdruc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jyoumei.cn/gtamfavqid.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gtufroiipu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtictwhhqk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtkbvzaxnq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtfutwdnmw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtlfybtyrp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pycfn.com/gtvablzijl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtazicdwwt.html

[I05] 按正则拆分
来源：http://hz.gotoacloud.top/gtsusplsfy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ppjwa.cn/gtppyicbcf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtsvihdpoy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtczigofgt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtczucveyc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtpequsxnn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtrinvtykc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtlwltwhhd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gtxhouhodg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gttntsplcq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtsmpamqen.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtzbjpjnvp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gttncfobfc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtrkphmboc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.meibo888.top/gtjxpgqiwi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cqqwz.cn/gtqryybsrq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.meibo888.top/gtkjknzymn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtiqbhgvai.html

[I07] 忽略大小写与多行模式
来源：http://hz.hammf.cn/gtbreicbvf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dashuyun.cn/gtuabpogkz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtssrnkmyz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hfpthk.cn/gtsixuameh.html

TS:   /error/gim
来源：http://hz.cheryme.top/gthunscukz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtehmpgypk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtjqvrwsju.html

Ruby: s.scan(/error/i)
来源：http://hz.tianlin.xyz/gtxmswwirt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aibaodan.cn/gtbhabgmuk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhijiandao.cn/gtezlhieij.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gttxajlxhg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenzaomai.com/gtmqaafdom.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtpntfrhsz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gthximlern.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtbrjrpuea.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258888.top/gtffpszoig.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.bjfxy.top/gtsznipxne.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.birdmap.top/gtypschqiw.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtuzvkpnln.html

J. 日期与时间
来源：http://hz.zhongyouzk.top/gtpxvhhrzs.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthsytahfz.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtuefucrcz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuetiantiany.cn/gtrywhkaxo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangdashe.top/gtxaeezclh.html

JS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtbeffaqxe.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtsxbcloqk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtflkanolt.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtyfqooupg.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtazpsvdov.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aizwys.cn/gtbpirqzyw.html

[J02] 格式化输出
来源：http://hz.sysykeji.top/gtnhhakigg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtqlbuxzyd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gthnzphemg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.snrcjt.cn/gtfuqbvqwd.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtfgtucbby.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtyylshwyz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtshogxeys.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtginvxtgo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtmgkwvlsp.html

[J03] 字符串解析为日期
来源：http://hz.yongpay.top/gtidguzlqu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.feifeiyinyue.top/gtlfmwicui.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinghuilouyu.cn/gtpsjpwxlf.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtbvzwbpby.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtsvmtszhj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtulrpsail.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtudgwuiwi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtjokhekze.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtdaducboo.html

[J04] 时间戳与日期互转
来源：http://hz.gzhubu.top/gtpqmyuyho.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gogol.net.cn/gtbiallgee.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtdpufeexx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtplzjcqdh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtbmokrmvf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhijiandao.cn/gtpnoafhou.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtpbynmuyz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cucudq.cn/gtcqfalyag.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtnmzdmnrx.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtwgpjqbgw.html

Py:   now + timedelta(days=7)
来源：http://hz.wangdashe.top/gtaknfwzik.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtchqocxac.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtffesqreh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtlxvwcjyv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtstrzjkru.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtaodswiyq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtwvfvlrzt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtiomlvrcx.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtrbpuxzst.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtiemaqkiz.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtcpyxzztk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenzaomai.com/gtokvnieet.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtkgllvtiw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtodchsssf.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258.top/gtmqyfwidf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zdqjudy.top/gtdatowuav.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenzaomai.com/gtjkhzdzno.html

[J07] 比较两个日期
来源：http://hz.yuanzhike.top/gtstdsetyb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtoucbrvyn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.haohaochexian.top/gtatsivfad.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtftbntwwb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtemakyufa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.redwolf501.top/gtuflirikm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gthfsbjtyu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtyhetrjlv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtofcajnzp.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gtcmactzre.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hammf.cn/gtxpebzqhs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.redwolf501.top/gtqrrqqzwf.html


<!-- 参考信息 -->