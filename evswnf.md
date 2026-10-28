代发 wailian999

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtoyzvjray.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtwwzuxdoe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangtech.top/gtmlitzkyv.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtydsxcrzx.html

C#:   public / protected / private / internal
来源：http://hz.ivvv.top/gtsgctawon.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtguuelqoz.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtsjzrwfzn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtxccltcwb.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gtqgtjvdtp.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gtzuroiffm.html

Java: public String getName() { return name; }
来源：http://hz.xylfe.cn/gtikmkikqj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtfqoozhsj.html

Ruby: attr_accessor :name
来源：http://hz.jinqigfzy.top/gtfbfewpjs.html

C#:   public string Name { get; set; }
来源：http://hz.ydjk.org.cn/gtkcijgmrl.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtfcczkzsq.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtdbtbdlgn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtphflcoug.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtpvnepqcn.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtomjmfcic.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtstzxjihg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtuvxveome.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gttgwuuvxb.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gthoslnjsq.html

[G13] 判断对象类型
来源：http://hz.cdnleiting.top/gtqynucfwa.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtbiohescf.html

PHP:  $u instanceof User
来源：http://hz.bjfxy.top/gtyjiubdnj.html

JS:   u instanceof User
来源：http://hz.chenlongwang.top/gtdvkxquov.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtpdcbrudd.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtsvaybziw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtfsusfwky.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gtxifaokha.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtiunlalur.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtrepdnjgt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ppjwa.cn/gtdrijqmqz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhongyouzk.top/gtfepfusrz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtyihnpjuv.html

TS:   type User = { name: string; age: number };
来源：http://hz.cqqwz.cn/gtmnsnwhvg.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtvcfprmwz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.quarkkingdee.top/gttpavwtdw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtepjdstaj.html

C#:   record User(string Name, int Age);
来源：http://hz.9152youxi.cn/gtsqyprhfn.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtyeuncvxv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtdrbcpadt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtzmheqixq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtwovxuege.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtthduiico.html

Java: enum Color { RED, GREEN }
来源：http://hz.shuidangran.top/gtxuonzgof.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pengpengdd.cyou/gtumeissah.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtfjunjkzs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtwbsemihb.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtlzxjzqgk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtgsokfrwn.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtzykspzwt.html

JS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtmgjxhbtk.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtifwogjlh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ywan-chungtsiang.top/gtiqpmnnqo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ehwqpu.com/gtxpuqwffq.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gtloggprta.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tianlin.xyz/gtdpzvjvsg.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdzozsceo.html

H. 异常与错误处理
来源：http://hz.hfpthk.cn/gtrqaknera.html

================================================================================
来源：http://hz.bjfxy.top/gtpugatzns.html

[H01] try / catch 基础
来源：http://hz.chenjidiqi.icu/gtkhxjjxur.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenlongwang.top/gthxybcznn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ybcxt.top/gtuflavhut.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.redwolf501.top/gtbyyxozte.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtutrfazpd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtthwsoagq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.mhx1999.top/gtjifyjrep.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jyoumei.cn/gtszzdvmgh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuanzx.com/gtsbwdwtfk.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtsseqsvnc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtgznhhzbk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtqjnxmfgl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtjptoglxh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gthlmwrsje.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtoesyfkyv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtsorddnxj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cucudq.cn/gtsgzyqqxb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtflpaceof.html

[H03] 主动抛出异常
来源：http://hz.smart0.xyz/gtofosbjyz.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigfzy.top/gtdiwosrpl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtspuimxii.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtlrjhqnmj.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtfuwhtmyj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtevvhatrl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhaomingkeji.xyz/gtvvfxpxhd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtyqhhxoyt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtjmwlxnjk.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gtlhtjckjq.html

Py:   class MyError(Exception): pass
来源：http://hz.daria6918.cn/gtyjkbrlih.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gteoovupha.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gthwdaviej.html

TS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtusiewsoy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtdgzkozwp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gthvuijgre.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtchxjltfv.html

C#:   class MyException : Exception {}
来源：http://hz.hysaishi.cn/gtkvwxwelt.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtheqdzdlw.html

Py:   except ValueError as e:
来源：http://hz.vqdsnc.cn/gtiseibxvd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtgxpcqxct.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtdlbdprib.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtwyjyzbbe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fengsongda.top/gtbmrdqjyx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtnkanqzyd.html

Ruby: rescue ArgumentError => e
来源：http://hz.haohaochexian.top/gtmflezxnk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gtjnrfxtsh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gtmjjdsiqw.html

Py:   value = d.get("k") or default
来源：http://hz.ivvv.top/gtrfnxqsue.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtiqhdnawi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtecfbvrga.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtyzgayvkf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gtajeaynzb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gthhzbmuml.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gttknahuuf.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gturkfgewq.html

[H07] 断言
来源：http://hz.andypj.xyz/gtqkvccbqo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cheryme.top/gtnttmsosl.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtjwhmiojc.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtzihuossi.html

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtcryliwep.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cheryme.top/gtgvdnqypy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guannengcc.top/gtlzkrkebh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daxiang520.top/gtpnshutdn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yongpay.top/gtteeqmogz.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtfojuywxt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgfzy.top/gtpvnxmqoe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cashguo.top/gtmvcklvae.html

JS:   e.message;  e.stack
来源：http://hz.tian-w.cn/gtszoahjtl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtofrayxnq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxinkj.top/gtankubtxs.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtacktvtsr.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gtvjvblocl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gzhubu.top/gtxrqncjyo.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtrezuymvm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yangfankeji.com/gtafhudnzd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtvraruaah.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gtlhohfjgf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtctdzkqve.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hfpthk.cn/gtmsldgnco.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtlnzaabuw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtgnpbsdky.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gtovuspjsc.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gtllusfekm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtoitimpzb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gtmroahufu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtihvwssei.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtunttdvpd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hammf.cn/gthbuafeea.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtghosnaig.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtjbxprniw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gthptyzyjj.html

================================================================================
来源：http://hz.guowangkeji.top/gtgyiswcjq.html

I. 正则表达式
来源：http://hz.yj20258.top/gtfkfcggba.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwxkmhpnq.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtzkacscyo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ppjwa.cn/gttagauclt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtzxdnzhxr.html

JS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtiiabdgfl.html

TS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtypytiqmj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gthgshdria.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtyuxlowzs.html

Ruby: s.match?(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gttsdimfxa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtlzyxoqzm.html

[I02] 提取所有匹配
来源：http://hz.shangyingyoupin.top/gtgyfqjmwf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtbswoofmh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtueatfgjb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhixingplan.top/gtgndoiuex.html

TS:   s.match(/\d+/g)
来源：http://hz.gogol.net.cn/gtoroznkpm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtrfnxbzwz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtbgicudcp.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtfsdleaub.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtlfxphhfa.html

[I03] 提取捕获分组
来源：http://hz.ppjwa.cn/gthbrybwbk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtfeqphvce.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xylfe.cn/gtkquzlevk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dashuyun.cn/gtezzywvws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gzhubu.top/gtonufbgtr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.316326.xyz/gtvxlktldo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenlongwang.top/gtqaynabiw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.meibo888.top/gtmanpjalb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.svipenyu.cn/gtunmwazez.html

[I04] 正则替换
来源：http://hz.fengsongda.top/gtyfefoxkt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtldqombus.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daria6918.cn/gtttagpflp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtuqurucaq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtvbiwfigs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtmguqxcff.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shzxlz.cn/gtntbfyrhb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj202588.top/gtrzdpissr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gogol.net.cn/gtkgnbytxy.html

[I05] 按正则拆分
来源：http://hz.jinghuilouyu.cn/gtwkpzcpac.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtxymeidgo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.smart0.xyz/gtykxsdvee.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtebwurard.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtzdnhonfj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258.top/gtyckdjnee.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.feifeiyinyue.top/gtntzeiqqn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtryhhbluv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gtdgffdjmx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gtmwbdxyfy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtzszmjfzc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.9152youxi.cn/gtkohbxpnz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtomkqztbj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtdpzaedop.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jianghu66.top/gtnvgmhhul.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.feifeiyinyue.top/gtoudugxrz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jyoumei.cn/gtwejguwnq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtwxuokbqn.html

[I07] 忽略大小写与多行模式
来源：http://hz.iojbl.cn/gtlrshzyde.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gthqarqcwq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydjk.org.cn/gtjgqbkhuq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtqrbydjnj.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gthgtknnhb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhijiandao.cn/gtujemviwj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxuanxn.top/gtnkfhywxe.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtnqnsbbmd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenjidiqi.icu/gtovfvihim.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtpccmuxwq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtsphqlrah.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtizqulkvx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtrqxdujct.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtbwhxvrds.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtwmfvaudo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtjqrnrldh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuxming.cn/gtwenukfwk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtoqsknnkq.html

================================================================================
来源：http://hz.tianlin.xyz/gtwnfqejdn.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gttexrgwau.html

================================================================================
来源：http://hz.guowangkeji.top/gtsfjewais.html

[J01] 获取当前时间
来源：http://hz.shuidangran.top/gtrqaedptv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtrvgllesu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtmesfbftq.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtwekhwvsn.html

TS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gthgyhysnp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtwtdfatwk.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gttffoyufc.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtovqvrszs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuetiantiany.cn/gtvfehyfrt.html

[J02] 格式化输出
来源：http://hz.hywenlv.cn/gtldpujxkq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtdaijpxpn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtleotqnxc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtusyaxmck.html

TS:   d.toISOString()
来源：http://hz.meibo888.top/gtycapmmqt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenzaomai.com/gtrznzhipm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtkiqsiewm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtwpqktbya.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtrgtqbbqc.html

[J03] 字符串解析为日期
来源：http://hz.hnxiangtu.top/gtndnjtfmi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtqvqsncjb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtdavezexu.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gttonuajqy.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtladksijd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtspuhuccw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gthjrlfxkx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtdkcopzij.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtndgylblc.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtgmomcjuo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtwbhajiru.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gteajeogqn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtkkzcuihe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gteeseuuzr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.c1oappe.top/gtacyuwdup.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinyuanbaomall.cn/gtvpkbasqu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenjidiqi.icu/gtwqkyouqt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhixingplan.top/gtvdmmvmpc.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtcxicvtzk.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtmuncrdsx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gaohongyu789.top/gtsoweejaw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtxmtwmvuw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtfmxktewa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgfzy.top/gtjrpegvmj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sufxvd.cn/gtjgvsisqo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gtiqkqaruy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cucudq.cn/gtmcvaeaos.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtbuyxszky.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gtphwwgbjl.html

PHP:  $end->diff($start)->days;
来源：http://hz.redwolf501.top/gtbqmjzrca.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jianghu66.top/gtwnegidjh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.9152youxi.cn/gtqijddtkq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtxbdzvwwb.html

Go:   end.Sub(start).Hours()
来源：http://hz.dashuyun.cn/gtcqssshem.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258888.top/gtixmipcvw.html

C#:   (end - start).TotalSeconds
来源：http://hz.meibo888.top/gtvwxjfhbw.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gteeuwnwuq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtadpcszjo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gtdtzvxdpd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtvotzuymc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gthphdszyp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtaodbnfai.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tanke756.top/gtaofpjzsu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtcgybgkke.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtmxiyaqtq.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtyycskufs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jiagoushi.top/gtohfuwyfw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtlfxkcuih.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtkfmpscaz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtzxzynzxc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dashuyun.cn/gtsrqgvzuh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yanxiufei.cn/gtwujnsnqy.html


<!-- 参考信息 -->