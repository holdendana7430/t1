代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gteowkdthx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgufenzy.top/gtsaccxaye.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuanzx.com/gtoyggjxcb.html

C#:   interface IShape { double Area(); }
来源：http://hz.guowangkeji.top/gtobwjjhxg.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtwycmsoyg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtbxgngbml.html

PHP:  public / protected / private
来源：http://hz.gogol.net.cn/gtrjetciyf.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtvbzrfdry.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtescdgorj.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gttytrrgrk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtnniimcmn.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtdacpspcf.html

C#:   public / protected / private / internal
来源：http://hz.sufxvd.cn/gtczhjxact.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtwyfmacom.html

Py:   @property 与 @x.setter
来源：http://hz.xziqi.cn/gtbpjxkuom.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtebyqbjzg.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtxqeatbim.html

TS:   get name(): string { return this._name; }
来源：http://hz.xinyue.icu/gtzwtlkmzf.html

Java: public String getName() { return name; }
来源：http://hz.yongpay.top/gtvputrnwa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gttkyrecrp.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtsbyhevfi.html

C#:   public string Name { get; set; }
来源：http://hz.yj202588.top/gtcgtrwezy.html

[G12] 对象转字符串
来源：http://hz.ivvv.top/gtojpufyxa.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtzzuwngyw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtpeyfearp.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gtqoqrvqfr.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtbwbsvmri.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gttagpmwbd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtksfyznjz.html

Ruby: def to_s; @name; end
来源：http://hz.pengpengdd.cyou/gthhnummgw.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtzpxufbkf.html

[G13] 判断对象类型
来源：http://hz.gogol.net.cn/gtbixxjubl.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtqnmyalhd.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtaevmuwyw.html

JS:   u instanceof User
来源：http://hz.aibaodan.cn/gtwkkcmxgx.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gttbmigzju.html

Java: u instanceof User
来源：http://hz.gogol.net.cn/gtfdzlvynw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtjaxxmiuh.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtepjhkbak.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtnaqyaokr.html

[G14] 数据类 / record
来源：http://hz.ivvv.top/gtnlmgkyuo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtyruppzwq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtfhzcpbto.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ywan-chungtsiang.top/gtenvtunib.html

TS:   type User = { name: string; age: number };
来源：http://hz.ehwqpu.com/gtqkxdlsge.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtsbdkywhb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtqxtohlxk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtuleqozbf.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtdoghzkqx.html

[G15] 枚举
来源：http://hz.jianghu66.top/gtrpdcfuns.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gthhtadeim.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daxiang520.top/gtbjfvsduv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgufenzy.top/gtqdbmdrxm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtmvpfsbwl.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtoxhkzfkj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gthztdiyki.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangshuangyany.cn/gtnlhsigsm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtxoviwflt.html

[G16] 对象转数组 / 字典
来源：http://hz.xuanzx.com/gtvmkycvtc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.andypj.xyz/gtirhiyfbp.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtghluhbda.html

JS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtlywzlwaz.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtwqrcwetx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shuidangran.top/gtegposdkf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gtivulvisr.html

Ruby: obj.instance_variables
来源：http://hz.zhongyouzk.top/gtunmmvzlv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtgqltljvu.html

================================================================================
来源：http://hz.jyoumei.cn/gtzmahtmjj.html

H. 异常与错误处理
来源：http://hz.haohaochexian.top/gtjbjkbrbg.html

================================================================================
来源：http://hz.hnqzz.top/gtuvebjlkm.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gthrmtwpdn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.iojbl.cn/gtyjctmrsq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shangyingyoupin.top/gtpccvsqqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtldivphck.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.svipenyu.cn/gtiofbzhqp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuanzhike.top/gtdblekiwh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gtuubegxrt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhixingplan.top/gtupmevjte.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtgeopfvpe.html

[H02] finally / ensure 收尾
来源：http://hz.gogol.net.cn/gtgktdvjnp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gzhubu.top/gtrkkqulev.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtdjawjhvq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtxzykemrb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtxrvccovu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtefxcrnmo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtdqhbwwbo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtfkunzuny.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtjxrbnfja.html

[H03] 主动抛出异常
来源：http://hz.fengsongda.top/gtngbfcpxu.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtqndydifo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtqvybvxjb.html

JS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gttkqmfshr.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtygjphlka.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj202588.top/gtovjmtzuf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gtozujqnzy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dashuyun.cn/gtkpncpnfi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtuhgtrdvy.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gtbzpellzf.html

Py:   class MyError(Exception): pass
来源：http://hz.vqdsnc.cn/gtgedcwvbi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtmsjpentz.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtbzminocj.html

TS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtycmzibnf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gticwgoamg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtfwenirrp.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxinkj.top/gtqikjnaxp.html

C#:   class MyException : Exception {}
来源：http://hz.jlsjyb.cn/gtlkfkbdfn.html

[H05] 捕获特定类型
来源：http://hz.ydzc1.top/gtgqospwxv.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtsintwaje.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtuupwmwsc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtcoqkqmmz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtvihjzqet.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtajpzlpom.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.kuanghao11.cn/gtzwwmtrpe.html

Ruby: rescue ArgumentError => e
来源：http://hz.shangyingyoupin.top/gtnijgjunl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.0kj1m.cn/gtxxkztpex.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuanzhike.top/gtwyvkszfq.html

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gttwbnnxix.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhongyouzk.top/gtuclcnmye.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtldidotwp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtowvqpuia.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ivvv.top/gtypdbxwdf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ivvv.top/gtirajipjs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtdunreatn.html

C#:   obj?.A?.B ?? default
来源：http://hz.cqqwz.cn/gtuemztfnj.html

[H07] 断言
来源：http://hz.cucudq.cn/gtkzagxlhy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yongpay.top/gtrksvafhg.html

PHP:  assert($x > 0);
来源：http://hz.haohaochexian.top/gttorckfra.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtmyktmiqx.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtjcvhpnho.html

Java: assert x > 0 : "必须为正";
来源：http://hz.smart0.xyz/gtaqvautxs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guowangkeji.top/gtdlirkajt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gtnyyneave.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258.top/gtiesenxgx.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhongyouzk.top/gtrfjsrbdi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtjwsozmqa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgfzy.top/gtlfcuuhpm.html

JS:   e.message;  e.stack
来源：http://hz.aizwys.cn/gtqcucjniv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shzxlz.cn/gtqxgwmdtg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtyhfhjyvg.html

Go:   err.Error()
来源：http://hz.zhaomingkeji.xyz/gtcrwrmshp.html

Ruby: e.message;  e.backtrace
来源：http://hz.feifeiyinyue.top/gtgpccgaas.html

C#:   e.Message;  e.StackTrace
来源：http://hz.smart0.xyz/gtpbemamob.html

[H09] 带错误码的异常
来源：http://hz.zhoulong.xyz/gtxuzxkocj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtcnwpqlgk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuxming.cn/gtohokopbq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hywenlv.cn/gtrzajtoqw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgfzy.top/gtvdcmiznj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gtqcxpsrsy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gtejgnndai.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtfceydrqm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gthilcexvh.html

[H10] 资源自动释放
来源：http://hz.gzhubu.top/gtmfrtvivr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtrtlozids.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gtwsjhcoti.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtbniweolq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtcgkzlvub.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtfqwarljq.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gtausugjet.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuxming.cn/gtvcbmykpn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.snrcjt.cn/gtkirlrqfq.html

================================================================================
来源：http://hz.bjfxy.top/gturjowzpp.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtluevvnvu.html

================================================================================
来源：http://hz.havefunace.top/gtyqfjrumz.html

[I01] 判断是否匹配
来源：http://hz.smart0.xyz/gtoidpyvze.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtebtpwsjj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yonumen.top/gtvpqtmvfg.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtldfbfugt.html

TS:   /\d+/.test(s)
来源：http://hz.316326.xyz/gthkwkvkaw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shzxlz.cn/gtjazmxpwi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtrhbnkrhu.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtmoqggesi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtwomcivae.html

[I02] 提取所有匹配
来源：http://hz.ybcxt.top/gtglizlilv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtcwttbemr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtuawwqkur.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gteeqczffb.html

TS:   s.match(/\d+/g)
来源：http://hz.zhaomingkeji.xyz/gtjbhbcczh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gtmtkglqay.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gteyskcafu.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtehsmyidm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtdwrxebbi.html

[I03] 提取捕获分组
来源：http://hz.shzxlz.cn/gtanvvgnud.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtlcgcbdxl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258888.top/gtwqbjzhan.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hywenlv.cn/gtzzonwcfm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydjk.org.cn/gtigndykzh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtrgccvsjy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yangfankeji.com/gtwssqtqaj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gthkovgqng.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtnidfvnrh.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtdaqhccmq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nwbrower.top/gtelcqayio.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtgtnwgtko.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtnmjpgdrj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtavrywium.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gtlkxmbzcg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinyuanbaomall.cn/gthsrtvsux.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtypzxvoio.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.bjfxy.top/gtyhjihjkd.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtvpzjkymw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dashuyun.cn/gtrjmofxwv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pengpengdd.cyou/gtzxjluolq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtresoqlvy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtgcnkkvuw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtimmqxtuu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtqualueir.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtpocbsnsw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.mhx1999.top/gtrjgzshkb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shzxlz.cn/gtciwhacbf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtuhwnrahq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtltbtskyf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtmdzhbdsf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtoziiemfw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtfmelixjk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtgiazmpid.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.9152youxi.cn/gtfeyelojh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtkbrigvjh.html

[I07] 忽略大小写与多行模式
来源：http://hz.cashguo.top/gtsoytisye.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtnnxwktxj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jiagoushi.top/gtymwbtmys.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtwrdmvabz.html

TS:   /error/gim
来源：http://hz.xziqi.cn/gtuflriujt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtfscdkmbd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258888.top/gtcrahydbt.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtfhmkeesk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxinkj.top/gticdvdhbq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yvedp.cn/gtrdcwgnnj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnqzz.top/gtoadcltku.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.kuanghao11.cn/gtmlnjaxds.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtwwzpxsbm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtyzcojhol.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sxryk.cn/gtrgstczaz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtgyqhzwqh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shzxlz.cn/gtezpgifye.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtmpkvzkcm.html

================================================================================
来源：http://hz.ehwqpu.com/gtewnnsgqx.html

J. 日期与时间
来源：http://hz.ppjwa.cn/gtfryuxguc.html

================================================================================
来源：http://hz.daxiang520.top/gtuvayfpih.html

[J01] 获取当前时间
来源：http://hz.sufxvd.cn/gtqkbcddtt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daria6918.cn/gtsondkzfk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtyakjnahx.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtdrlnscuv.html

TS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtmfaedflg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtbomiefvc.html

Go:   time.Now()
来源：http://hz.gotoacloud.top/gtabyrhgrb.html

Ruby: Time.now
来源：http://hz.havefunace.top/gtfskvjafp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtuyyeayuk.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtgwvikofd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtrxaxkhqw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtdimoawny.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ybcxt.top/gtyntpfnug.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gtzvipdhiz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gtwfolgxlt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtucbojepv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtkqotbsqq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dianchejie.cn/gtgevqxuyi.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtvzkrmvbs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shangyingyoupin.top/gtqpqfzhzj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.smart0.xyz/gtdqecevvs.html

JS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtkykckxfz.html

TS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtiskvytjs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtrunfgacx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigfzy.top/gtusczngjk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gthodhtxjx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuetiantiany.cn/gtmjfnqxcc.html

[J04] 时间戳与日期互转
来源：http://hz.nanxuanxn.top/gteojrfoxv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtwrnqvgfe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.0kj1m.cn/gtwhfvcdkf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtqkzrtrcj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtpyehqitf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.bjfxy.top/gtcmrdzfyz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtnogmzllp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtgbswuhak.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtjnfhcwza.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtnuvrjxro.html

Py:   now + timedelta(days=7)
来源：http://hz.zycfv.cn/gtsyjdooen.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtbeytuert.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtvngwpiyr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtadacmclm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtajrrcclc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gtjpdsksux.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtxmuavzje.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gteazrgmyy.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gttrhudeav.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtfqninlpy.html

PHP:  $end->diff($start)->days;
来源：http://hz.hysaishi.cn/gtklvszwet.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gtbzbuaayd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhongyouzk.top/gtyrztksno.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jiagoushi.top/gtoydifdkr.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtsdmlijjb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtsypcchdw.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtgculxovp.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtjtlltntf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtgpwarrzo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenzaomai.com/gttwxteqov.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtosoqhety.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtbuzoyquv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.svipenyu.cn/gtpsfspiay.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenzaomai.com/gtxtfcxdyi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtiopqxtir.html


<!-- 参考信息 -->