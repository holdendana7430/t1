代发 wailian999

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtjhimhihf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gtcfucabck.html

PHP:  public / protected / private
来源：http://hz.xuanzx.com/gtxsmmjizd.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtaofrogwi.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtivtdzwtb.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gtlyukegzy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtigxrujmw.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtgrpujnes.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gttfvmzirc.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtxtuqazox.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtcshcralz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtynxzkikk.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtluftangr.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtetskjhrd.html

Java: public String getName() { return name; }
来源：http://hz.xuanzx.com/gtrttjzyjw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtckuyzbfi.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gthgfvawbw.html

C#:   public string Name { get; set; }
来源：http://hz.snrcjt.cn/gthquoimfs.html

[G12] 对象转字符串
来源：http://hz.52xcode.cn/gtyxuulqhh.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtvfrxeqhm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtsqiykbwe.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtecgwqxny.html

TS:   toString(): string { return this.name; }
来源：http://hz.nwbrower.top/gtogulycqk.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtdygxnbeg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gotoacloud.top/gtmwqiidhk.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtkruriyky.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtofeehpyd.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gtmnrwfwac.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gtgdhbowbn.html

PHP:  $u instanceof User
来源：http://hz.daria6918.cn/gtvtqlrffd.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtohidldhj.html

TS:   u instanceof User
来源：http://hz.pycfn.com/gtndoygolk.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtxxxedobd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtvbfcktsl.html

Ruby: u.is_a?(User)
来源：http://hz.316326.xyz/gtrduwedus.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtycbjavbl.html

[G14] 数据类 / record
来源：http://hz.shangyingyoupin.top/gtftxanwzf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtbzlpooss.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnxiangtu.top/gtkhcfmrav.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtppttbeet.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtrctdldrz.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtpwztowrc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtbjvxkvxs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtmgxcvzaf.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtiktagaav.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtopvxlopv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtdoueljfu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tanke756.top/gtlofwpctj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aizwys.cn/gtsknebdvj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtgcuvaviv.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuanzhike.top/gtmmzkimol.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtiofhgmhn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aibaodan.cn/gtfbuwaysr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtleohampn.html

[G16] 对象转数组 / 字典
来源：http://hz.316326.xyz/gtchysczna.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtpkuoftic.html

PHP:  get_object_vars($obj);
来源：http://hz.jlsjyb.cn/gtkamouxra.html

JS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtrtsvnuit.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtvvqnppgw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtwjojzmcw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtvvsmvvuy.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtnkvdakxh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtfogsollv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtkphsoiqb.html

H. 异常与错误处理
来源：http://hz.pengpengdd.cyou/gtdrkordmj.html

================================================================================
来源：http://hz.ppjwa.cn/gtyogoocqr.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtrgvmqrzx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gttpwwlpko.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinyuanbaomall.cn/gtseqxnjhr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gttgdrqsah.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtzjdfclrd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtnrxohuqz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gtponrdttw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtfhggsqsz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtdixzlzqi.html

[H02] finally / ensure 收尾
来源：http://hz.cqqwz.cn/gtelyuzcdp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.vqdsnc.cn/gtqahgckzm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtyiqtgolc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtdlgfniwz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtcrgmjuwc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtxkvjyxek.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gtznjynmeo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xinyue.icu/gtujowimhz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtrgjpwbme.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtfrtgbbuq.html

Py:   raise ValueError("错误信息")
来源：http://hz.cashguo.top/gtmmadiofl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtamrgjdxo.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtmqdmurzp.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtsrhcdzns.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtladwqcxg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnxiangtu.top/gtiocvcxuv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gtjezjzzuw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gttfmujaev.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtvutcwdqs.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtpbtbigrg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtehorklqw.html

JS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtpdsiurzi.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtqhduzllw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtlqfwgaoy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangdashe.top/gtyhpweoby.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gtwavcikkt.html

C#:   class MyException : Exception {}
来源：http://hz.cashguo.top/gthxrdlssq.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtuqzfhltf.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtanuiscwx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jyoumei.cn/gtnbfjitqm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtmwrgwjhn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtuiqecpks.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtsngbhzee.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gtcvcrclyf.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtkfexkpss.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtataltbvg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nwbrower.top/gtrdwhdtqx.html

Py:   value = d.get("k") or default
来源：http://hz.cqqwz.cn/gtdqzupemh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtvaejdehk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtoecmpbps.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtvdhnmjui.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtgzutrvjq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jianghu66.top/gteqpdlgga.html

Ruby: d&.dig(:a, :b)
来源：http://hz.kuanghao11.cn/gtaetudabw.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gthpajgjop.html

[H07] 断言
来源：http://hz.aibaodan.cn/gtfcqdfsmb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pengpengdd.cyou/gtxqlkehza.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtxqktgqmo.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtjdlqapkc.html

TS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtpalgomqv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sxryk.cn/gtddgippza.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yonumen.top/gtifmuiqvj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtpztrzlno.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tianlin.xyz/gtpmwsqsre.html

[H08] 获取错误信息与堆栈
来源：http://hz.shuidangran.top/gtishphesx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gtbkdyeadh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.316326.xyz/gtcrpedtcz.html

JS:   e.message;  e.stack
来源：http://hz.jqgfzy.top/gtdkuigbmh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtrghmolse.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yanxiufei.cn/gtqmuyoazu.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtonznpunk.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtbxdkikkw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sweek.top/gtlbjqlpoa.html

[H09] 带错误码的异常
来源：http://hz.yj20258.top/gthfwfocob.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gthujyrnbn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnqzz.top/gtpndbbhcg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gthqqpwamn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtuekhglfx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtdwstrczn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.kuanghao11.cn/gtchyrtrdb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtdqkbnnpb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuetiantiany.cn/gtkbybxpnm.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtatomdydd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ppjwa.cn/gteccfwlux.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gttciogwvx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtbyaduzzl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtfvyiqlfg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pycfn.com/gtpckjfsof.html

Go:   defer f.Close()
来源：http://hz.hysaishi.cn/gtswrzsudx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangdashe.top/gtxpallfbv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydjk.org.cn/gtyiretgzn.html

================================================================================
来源：http://hz.nanxinkj.top/gtksyhynpg.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtlcpogsyk.html

================================================================================
来源：http://hz.daria6918.cn/gtadcskqaj.html

[I01] 判断是否匹配
来源：http://hz.shzxlz.cn/gtbajypvax.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yvedp.cn/gtsepyzncm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtckzsvcxp.html

JS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtvzkiocor.html

TS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtetwjqvxt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fzhhl.top/gtxupxldai.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtgjbafgno.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtxigeachp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtvewrufnd.html

[I02] 提取所有匹配
来源：http://hz.hfpthk.cn/gtvtozzous.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtueropgda.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtuahlrxoq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtracsihih.html

TS:   s.match(/\d+/g)
来源：http://hz.shzxlz.cn/gtltxycdzj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gtdtfexuzl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtcgqxqsni.html

Ruby: s.scan(/\d+/)
来源：http://hz.pycfn.com/gtqedugsxi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnxiangtu.top/gtnzigqrpg.html

[I03] 提取捕获分组
来源：http://hz.haohaochexian.top/gtkytrqlgc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtrxafxlwd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sxryk.cn/gtfydaejxc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtksawzbui.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gogol.net.cn/gtxidvtxiu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258.top/gtuyzufexh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtpphasykz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtnkoncgfx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtdmqwnsba.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtuiqounms.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuanzx.com/gtrpwtcvrs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtfpimdkkr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtaqkhgdpd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtksubqoud.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtbldupjgt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yongpay.top/gtvayehvsr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangshuangyany.cn/gttbwosjjx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.andypj.xyz/gtzfoomwug.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gtcdcownpx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangdashe.top/gtjajunrmf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gtrewhkjcv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtmmvadvpm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gttikqkmgt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydjk.org.cn/gtgpzshwii.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtxbktrdjo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtnqpnewwm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtyuryybhx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtjzvkhnql.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtwfywptki.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtlnmepinl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtgoomkttb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtqlviuegk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sweek.top/gtxufrfrrw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtodozwmaz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtfyxsjoxg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.quarkkingdee.top/gtyjwwcwym.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258888.top/gtyxktrizs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtyfjcuelm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtbcnhhgsc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtufmplxgn.html

TS:   /error/gim
来源：http://hz.cucudq.cn/gtzonxvoaz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gttlemlsai.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhongyouzk.top/gtyfqhtwdk.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtidjielpw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.svipenyu.cn/gtqhyivfbg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gtpvebemei.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sufxvd.cn/gtcpbxnfki.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtucntzyry.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtgtxrdqge.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtinxdrgax.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yvedp.cn/gtrevumpvq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtdpwejzle.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtadbllekx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtgdsusbyg.html

================================================================================
来源：http://hz.sxryk.cn/gtqyfvzokh.html

J. 日期与时间
来源：http://hz.cucudq.cn/gtyzlvxgtk.html

================================================================================
来源：http://hz.hammf.cn/gtqpwhtpco.html

[J01] 获取当前时间
来源：http://hz.ydjk.org.cn/gtqqwkgtja.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.316326.xyz/gtbysqwysi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtuicrucdu.html

JS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtyxsmogpq.html

TS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gtjifmdifc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gttjvmpfcq.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtpjxcgjvp.html

Ruby: Time.now
来源：http://hz.gogol.net.cn/gtadmotvxx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtbmdhawuh.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtifcypjcg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtjnwgbccs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtasjpdjgn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtffrosoei.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtvefwcltv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258888.top/gtlgfcictz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nwbrower.top/gtspotnvvi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtmckomjhx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hammf.cn/gtxiieigjr.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtncrdvcft.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuxming.cn/gtjxlzzntd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtwirvvinp.html

JS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtwdrkgrbq.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtttkhvvjv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtzllammen.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dashuyun.cn/gtwyxoerhg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xylfe.cn/gttygmfqvv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cheryme.top/gtjwwmbspn.html

[J04] 时间戳与日期互转
来源：http://hz.sxryk.cn/gtdwryqcvb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtiqruhqnu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuanzhike.top/gtblkdfhtk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtamezkvdx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gtoxchjole.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtfgwqgotm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtkiyqwwhz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nwbrower.top/gtluogjfss.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtjvelubue.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtvnjujnpq.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtzppzxfdk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtuhpkfnnw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtgdgiayni.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtzlmcssvw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangshuangyany.cn/gtwapmpafx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtduryyaug.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gzhubu.top/gtahxrgaoc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtloeucthw.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gtswqjrepw.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtzhihadgp.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtrypimxtj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtfvijutxc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtjsowejro.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtyhkozwme.html

Go:   end.Sub(start).Hours()
来源：http://hz.9152youxi.cn/gtxbhmedjb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.52xcode.cn/gthtujcjym.html

C#:   (end - start).TotalSeconds
来源：http://hz.guannengcc.top/gthkedizxc.html

[J07] 比较两个日期
来源：http://hz.zhongyouzk.top/gtpndspnye.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtkcmfpndu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tanke756.top/gtfbharxka.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gtnnoqraux.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtzslimwpw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtjcjexqpt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jlsjyb.cn/gtndrramly.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtuxekkdqp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtajriukkv.html

[J08] 提取年月日与星期
来源：http://hz.yongpay.top/gtkvxgjblt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhixingplan.top/gtyfoubvst.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnxiangtu.top/gthrxfbihx.html


<!-- 参考信息 -->