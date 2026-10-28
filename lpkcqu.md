代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.shuidangran.top/gtdedytsxy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtdimbomsz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhixingplan.top/gthmuazpst.html

C#:   interface IShape { double Area(); }
来源：http://hz.yvedp.cn/gtjamrgooq.html

[G10] 访问控制
来源：http://hz.zhengqikj.top/gtbffiqgmd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtkjousrhq.html

PHP:  public / protected / private
来源：http://hz.yangfankeji.com/gtwplyuldj.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtsihdsslh.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtvqrjnvwm.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtqfjqrnaw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtdnyumitm.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtxypfjakg.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtuyegnukk.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtsmgioxgb.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtpnwxvdqy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtowlqmfsy.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtvxessvff.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gtmwmpmsqg.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gtleuyerjp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.smart0.xyz/gtzuqzlxbn.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtdrajvvol.html

C#:   public string Name { get; set; }
来源：http://hz.yvedp.cn/gttowyzufa.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gttlhozqdk.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtwgegnihc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ivvv.top/gtgylmiglu.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gtnrtjbjvu.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtdxovvpin.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtlchgcrkv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtcglkfqrv.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gtqxraveka.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gtujqkirfk.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtcubnsyiw.html

Py:   isinstance(u, User)
来源：http://hz.wangshuangyany.cn/gtceqimoap.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtgtmppwfp.html

JS:   u instanceof User
来源：http://hz.yonumen.top/gtcionvutj.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gteebxhemj.html

Java: u instanceof User
来源：http://hz.chenzaomai.com/gthhmdtrzl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtqpdvcajg.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gtvtxjnyra.html

C#:   u is User
来源：http://hz.birdmap.top/gtvevkaoea.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtwpgxsxju.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aibaodan.cn/gtgissooub.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.andypj.xyz/gtclgdzgoo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhaomingkeji.xyz/gtlkcnedua.html

TS:   type User = { name: string; age: number };
来源：http://hz.svipenyu.cn/gtyfofugte.html

Java: record User(String name, int age) {}
来源：http://hz.cashguo.top/gtbkeexqvz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.0kj1m.cn/gtivpadasx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dianchejie.cn/gtrjxiqkaa.html

C#:   record User(string Name, int Age);
来源：http://hz.aizwys.cn/gttzdshhhl.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtqfvuiixo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtsfsgvyje.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtdpqbjcbi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtnxtmiivm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtvebznouf.html

Java: enum Color { RED, GREEN }
来源：http://hz.andypj.xyz/gtqnbpeauh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.svipenyu.cn/gtzqwsnopy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.52xcode.cn/gtqfoalvfs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtmprxrytm.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtuadbkrar.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ppjwa.cn/gtnpbohdmn.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258.top/gtvhvhrgnu.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtqgwdsqxx.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtebjzbncw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtdhmkizwp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhoulong.xyz/gtrbenjlde.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtrcwcrbnl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gtraxilxhv.html

================================================================================
来源：http://hz.zdqjudy.top/gtouqzfkya.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtsiyphgmi.html

================================================================================
来源：http://hz.iojbl.cn/gtgmeudnsh.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtpcsdauar.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hongshengwenyu.top/gtukeealdu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtjkzivkbj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtxhagtsby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuxming.cn/gtiwabbics.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtphvtlrei.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.0kj1m.cn/gtrvehmrnl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gtpcjdlhom.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydzc1.top/gtwuabebjh.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtwsrdivak.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtybiomumg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtxqhhtlaa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gteuzyrlfs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtuybaskbm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtewnroapo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtxktnhvjd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gtwjtxpems.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtrkfbaufz.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gtwbssgdqp.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtmdlanfdc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtswcbryvn.html

JS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtcdegjexa.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtyzhxduow.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtpfguecue.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tianlin.xyz/gtuaitvayb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtvhtjcflu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtifpgmrok.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtbvprtrbx.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gtydfialvn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gttojhwinz.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtqwxgmgoc.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtjqitnktv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yueranfly.top/gtuebybjzj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cqqwz.cn/gtednhamom.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtetyhklku.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtvtjgtprm.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtmwiynuso.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtybmqndlj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gthxpzzhqo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtoxdlusbv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtocgazivi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangkeji.top/gtxbkqccke.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gteaatscat.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtcuevvvgc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dianchejie.cn/gtjxowkgcp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtacpvjcph.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtvazsrlge.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yangfankeji.com/gtwnvdcvjq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtsfoguwzi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtggybqamh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtrarwauxp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenzaomai.com/gtihrehpdj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.kuanghao11.cn/gtuhnaofua.html

C#:   obj?.A?.B ?? default
来源：http://hz.iojbl.cn/gtxpzqxvot.html

[H07] 断言
来源：http://hz.ydjk.org.cn/gtbgajtlsz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhijiandao.cn/gtqfgqfvtg.html

PHP:  assert($x > 0);
来源：http://hz.dianchejie.cn/gtkwfabfqo.html

JS:   console.assert(x > 0);
来源：http://hz.haohaochexian.top/gtoqppnggt.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtrdowkhgb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydzc1.top/gtpghbsyts.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhiwuduotai.top/gtfmdrynrw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.haohaochexian.top/gtiuqbublt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtddohfrce.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtolkwsxzi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtpngqmeqh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinghuilouyu.cn/gttajusroa.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtjcamhtdt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtmynlksbr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtszqmumdj.html

Go:   err.Error()
来源：http://hz.hammf.cn/gtgibiteor.html

Ruby: e.message;  e.backtrace
来源：http://hz.gaohongyu789.top/gtblbwoljk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtycscgpyb.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtinoldykj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hfpthk.cn/gtldlljvwj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtzrgtkfbd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtkkmcamtu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtkkrlpejj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guannengcc.top/gtfdmeyaft.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pycfn.com/gttzeoyjyi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtjpyazebj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtdbldnpuv.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gtgnpsrvju.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtxrowhyww.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ybcxt.top/gtaeafjyrf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtmyeccmzf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtcvzlyxyn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuanzhike.top/gtjyyforwl.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtpmicscfg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtzhvdoxih.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtixzqxwkt.html

================================================================================
来源：http://hz.gzhubu.top/gtbfetvhzk.html

I. 正则表达式
来源：http://hz.chenlongwang.top/gtsaetppyz.html

================================================================================
来源：http://hz.daria6918.cn/gtkxmbnngq.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtowhwmjtm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtflspqkrs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtxkqflqju.html

JS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtkallfrvr.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gteyerfmdd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtzyrqmlxc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtsnsynfzm.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gtqbniuihp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtdodiodjt.html

[I02] 提取所有匹配
来源：http://hz.sweek.top/gtgiqgwnib.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtessndybm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxinkj.top/gtijaouftm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gttjjaqlxw.html

TS:   s.match(/\d+/g)
来源：http://hz.cheryme.top/gtmbninwoz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtbdohvqlv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtwwccrcbp.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtzerjcird.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sweek.top/gtjlxjsgpe.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtayqdzmrt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydjk.org.cn/gtuyfwsfer.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtzxpocywz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ppjwa.cn/gturiczjsg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigufen.top/gtyncrzhqp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.smart0.xyz/gttwdrxwbr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gterykbxjh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtngieqllm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gzhubu.top/gtidtffbmj.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtztpjisxp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ybcxt.top/gtoqnvormo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtnmlhleda.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtiffbhxfs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtxajsrzvg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gteyrfhqrf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtpapzmqug.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gttpthmyhq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jlsjyb.cn/gtfogbmfbp.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtqbdwxqfp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fzhhl.top/gtguxzlvjo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtwdnwsixy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtzhjlbyza.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtskpyqfpf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jyoumei.cn/gtgayryzow.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gtsvxbyypu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gthphudhyp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtvdcowkyh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtjhwibkoe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtwzdfbsbh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuetiantiany.cn/gtbsiruvfw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gthppdwoqc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtljzxkjlu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtdrybthsk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xylfe.cn/gthrnqpggd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenzaomai.com/gttnupjnxn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtseduuzvb.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtahgnjjpb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.svipenyu.cn/gtumxkbqar.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtxopwdlrs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yongpay.top/gtcnidjdea.html

TS:   /error/gim
来源：http://hz.52xcode.cn/gtwmltffqu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtavhsayul.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sufxvd.cn/gtshdhcyil.html

Ruby: s.scan(/error/i)
来源：http://hz.cheryme.top/gtsrbvympx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fzhhl.top/gtpjdocrjs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.meibo888.top/gtftxweyvc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gotoacloud.top/gtrylsyiwa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gtbtvisrye.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtmlnmhzzi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtrevlwmki.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtqhwgvpli.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hywenlv.cn/gtqqjnujph.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tanke756.top/gtpjleatug.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gthtndzfyi.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtouaurmgd.html

J. 日期与时间
来源：http://hz.jlsjyb.cn/gtablmhovw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtghgsivka.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtwwzzbwfo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtgxtxybhx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtkrrygpxq.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtcbjihnqw.html

TS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtfnccczzh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gtlbvyejbn.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtrwymayev.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtwonsdjqm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cdnleiting.top/gtizkxrzez.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtridafvyz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtqbcbchym.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtpjrkhxpf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtplpgfypj.html

TS:   d.toISOString()
来源：http://hz.cashguo.top/gtbfiyyynd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gtqbxrcknx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shuidangran.top/gtawmshigz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtmksbtzjk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gotoacloud.top/gtnhcbffnu.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtvtooznal.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtkdmrdxob.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtrkmvchfp.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtrqitvuwq.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtcajchkqq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtzrqsbecf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.9152youxi.cn/gtbygdlcoo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtmveqmhhr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtshvphhgr.html

[J04] 时间戳与日期互转
来源：http://hz.snrcjt.cn/gtgblcwpgf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtprnuxrwu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hysaishi.cn/gthpnyfbvy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtrdqrmnfs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zycfv.cn/gtvjeodfxi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gtdfnffhve.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtbgnkfpwx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sufxvd.cn/gtysvfmtgq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cdnleiting.top/gtjpeocftz.html

[J05] 时间加减（加 7 天）
来源：http://hz.sysykeji.top/gtotsxtexb.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtjxmtlivj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtieaywvui.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gthksmcaww.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtdseuqbmi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtsjkacirv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangdashe.top/gtgypffstv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtrxrvlzwg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtnuldmqcg.html

[J06] 计算两时间之差
来源：http://hz.havefunace.top/gtepuoxdtl.html

Py:   (end - start).total_seconds()
来源：http://hz.guannengcc.top/gtcsgmsegc.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuanzx.com/gtcwztarac.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gzhubu.top/gtgxyqhtnv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gaohongyu789.top/gtcqarvfia.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgufenzy.top/gtaqgnjjdy.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtxtwknqjx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtfmahqcms.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtpexmpgws.html

[J07] 比较两个日期
来源：http://hz.zhaomingkeji.xyz/gtoblgorxe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtkklhtzmf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gaohongyu789.top/gtqnnkwths.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtbxubobsk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtjabpgwzj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtowlvwfei.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtthjiqzrz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtlqvdmqke.html


<!-- 参考信息 -->