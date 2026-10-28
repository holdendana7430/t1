代发 wailian999

[G10] 访问控制
来源：http://hz.zhoulong.xyz/gtzncnqdlb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinghuilouyu.cn/gtpikkcqxi.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtxgarudyl.html

JS:   #private 字段；其余公开
来源：http://hz.hysaishi.cn/gtjtlbyoxv.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtekvcdcet.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtpskktuni.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gtxqmkwvgr.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtdpffewsz.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtydcofqwo.html

[G11] getter / setter
来源：http://hz.pycfn.com/gtxqguclbe.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gtrnwkfxjl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtuaazzvnc.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtwfelwnnl.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtsvwvpvdq.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gtbhmascar.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gtomvealfd.html

Ruby: attr_accessor :name
来源：http://hz.yj202588.top/gteeuxkhkz.html

C#:   public string Name { get; set; }
来源：http://hz.jinyuanbaomall.cn/gtvmyfmhjs.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gtwxruhnpg.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtphtkkaxs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtgxqurmtf.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtnhjdlbaq.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtotiasdud.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gthuxbldpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gtelbfymyr.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtilysmxae.html

C#:   public override string ToString() => Name;
来源：http://hz.tanke756.top/gttvgdxbmp.html

[G13] 判断对象类型
来源：http://hz.jyoumei.cn/gtulpuzegb.html

Py:   isinstance(u, User)
来源：http://hz.hywenlv.cn/gtoikxreka.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtktblbrzs.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtjcbxcpho.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gttdeyfnma.html

Java: u instanceof User
来源：http://hz.zhongyouzk.top/gtvevadhsw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258888.top/gtpkkidwin.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtimxrjipz.html

C#:   u is User
来源：http://hz.nanxinkj.top/gtjydnpvza.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtgifzifcf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtuvnxaphv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.mhx1999.top/gtnehwofob.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtbzulstis.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangkeji.top/gtgjmyjbmg.html

Java: record User(String name, int age) {}
来源：http://hz.chenzaomai.com/gtafroejzv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cashguo.top/gthyzpcptr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yonumen.top/gtbjugezhs.html

C#:   record User(string Name, int Age);
来源：http://hz.bjfxy.top/gtlekjdvvx.html

[G15] 枚举
来源：http://hz.hammf.cn/gtyrxbpiab.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gtytilxpkt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtrgnejmzr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gotoacloud.top/gtgaoodjqg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtirpxphyk.html

Java: enum Color { RED, GREEN }
来源：http://hz.jlsjyb.cn/gtjcqknxgq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jlsjyb.cn/gtzejirzoo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtakycftpd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtupcazdif.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtkunyzkah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtxjacmjqq.html

PHP:  get_object_vars($obj);
来源：http://hz.jlsjyb.cn/gtyarvefsk.html

JS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtyzurtynf.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtzprldirn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtdgkyivmv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtizwqvjxo.html

Ruby: obj.instance_variables
来源：http://hz.jinqigufen.top/gtggrakfeg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xylfe.cn/gtycljmenn.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmhakmxxm.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtjfpjjbsw.html

================================================================================
来源：http://hz.haohaochexian.top/gtjpdfpmml.html

[H01] try / catch 基础
来源：http://hz.chenzaomai.com/gtcuwbfixe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhixingplan.top/gtfdvalevn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yangfankeji.com/gtcckzonvd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtjginhgnu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.meibo888.top/gtwzlttegy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinghuilouyu.cn/gtnlsmcuxo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shzxlz.cn/gtqmloabfv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuxming.cn/gttiskixec.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtrufsrwdg.html

[H02] finally / ensure 收尾
来源：http://hz.xylfe.cn/gtrqcadwgu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fengsongda.top/gttwbnkxjs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtdtnlvdky.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtjpsxhxpb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtxqaevott.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtmldeglmy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.havefunace.top/gtfwbyglxw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.feifeiyinyue.top/gtxfmlxpag.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gthjecoqnq.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtcurcubwm.html

Py:   raise ValueError("错误信息")
来源：http://hz.tanke756.top/gtplqqmkxb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtoykucxwu.html

JS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtttqjisss.html

TS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtntrzxhui.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtpslwscgj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtgofdvkrw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtyuxotocu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtddsbsbvy.html

[H04] 自定义异常类型
来源：http://hz.daria6918.cn/gtqcxmfoia.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtzusvumtm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtsdmbkzob.html

JS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gttemreccw.html

TS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtyzicceii.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtpeivznnh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtnhfssuck.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gthejpigyy.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtuuiznkqv.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtnkfwqirc.html

Py:   except ValueError as e:
来源：http://hz.dianchejie.cn/gtecgwvfsq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtkksvozpr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtgvbjdmvr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtqsuuqwnn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtycnizjdy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jyoumei.cn/gtgnkkkmmx.html

Ruby: rescue ArgumentError => e
来源：http://hz.9152youxi.cn/gtvtrubeei.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gthmrxffpk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtewniyvtq.html

Py:   value = d.get("k") or default
来源：http://hz.wangshuangyany.cn/gtgcfjttba.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigfzy.top/gtmgslkajr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gttrtvigws.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtolopyuyc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hongshengwenyu.top/gtzvcamnlr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jiagoushi.top/gtfhxligbz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sxryk.cn/gtvvxlsiui.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtippwtzzj.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gtmanajeim.html

Py:   assert x > 0, "必须为正"
来源：http://hz.havefunace.top/gtpfwcnxtg.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtdybaunoy.html

JS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtvlxmyojt.html

TS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gthgzbomkd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtacvnpprl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.kuanghao11.cn/gtahcieycq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtfoctzxho.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zycfv.cn/gtwefbkrwd.html

[H08] 获取错误信息与堆栈
来源：http://hz.daria6918.cn/gtcpzyoias.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ivvv.top/gtsvjnnqup.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gttojfbtsk.html

JS:   e.message;  e.stack
来源：http://hz.xylfe.cn/gtozqnieao.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gtbhgzuukx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jyoumei.cn/gtbyrmjewk.html

Go:   err.Error()
来源：http://hz.jinqigfzy.top/gtfwdmfdkn.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gtopzccsdl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtbvquljob.html

[H09] 带错误码的异常
来源：http://hz.cdnleiting.top/gtywcvajkl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenlongwang.top/gtpifjgady.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtdjomqzxh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtitidpmrz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yongpay.top/gtjkzasaca.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.feifeiyinyue.top/gtggmnodnv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tian-w.cn/gtfglzqcsf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ivvv.top/gttxsqpgvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtdiifxfcq.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtovehbmao.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.316326.xyz/gthbnelwgn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtoitmfmjm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtmynjeilv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtyydmhlwd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.vqdsnc.cn/gtpfpbevld.html

Go:   defer f.Close()
来源：http://hz.cheryme.top/gtarzrcqsq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj202588.top/gtlmxbiluy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtmqnfgxbq.html

================================================================================
来源：http://hz.hfpthk.cn/gtymvmwuiz.html

I. 正则表达式
来源：http://hz.sxryk.cn/gtsrchkkun.html

================================================================================
来源：http://hz.aizwys.cn/gttwxjwdxi.html

[I01] 判断是否匹配
来源：http://hz.yj20258.top/gtiskzyqen.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtnqsohbge.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guannengcc.top/gtncaohpmg.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtodnjnbwr.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtfndmwlmu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtvrkrcyvr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtgldshwbm.html

Ruby: s.match?(/\d+/)
来源：http://hz.zdqjudy.top/gtoetjnize.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtwalcnzij.html

[I02] 提取所有匹配
来源：http://hz.shzxlz.cn/gtywfndsci.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtasgcpeor.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtytqjvuxy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gtirgtfoff.html

TS:   s.match(/\d+/g)
来源：http://hz.zhoulong.xyz/gtzfpsgetm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtmwbigyel.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.andypj.xyz/gtcsxzukwt.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtucwzksik.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxuanxn.top/gtimxiucwj.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gtjfaqpjov.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258.top/gtmcyguwfr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtwnywwauy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.kuanghao11.cn/gtpdnhhupj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtdfkavnrl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtcrwiqsmz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtwrvwlhxs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangshuangyany.cn/gtblbofatt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dianchejie.cn/gtvnwjkspt.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtsqtywthl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gtsnrqhqnf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtbgnpunvh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtqldmnttd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtbkknvvlz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtmlapazcy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtgjslnjbu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtmubmylok.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.smart0.xyz/gtxstpmdhq.html

[I05] 按正则拆分
来源：http://hz.chenjidiqi.icu/gtjyfbmhmz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtkwlklnls.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guannengcc.top/gttepphteq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtrhcvpwlo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtkweqqdpy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtklhqllmd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gttrdedtcv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtabrhpxrf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xingfuxueyuan.xyz/gtmqnvubvo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtrwjpsxyi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtfomluyxv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.bjfxy.top/gtiyxcokdj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtqwyswepz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtvfszfrtl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtghxorqud.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenzaomai.com/gthrnmgved.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtgqetdzjs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtbrahjcaq.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtzfjhnufp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnxiangtu.top/gtvosffkxb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daxiang520.top/gtewbemovv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gogol.net.cn/gtfruswhln.html

TS:   /error/gim
来源：http://hz.zhengqikj.top/gtleoztjfj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtkwonazqm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sysykeji.top/gtvkdlicwx.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtooxnqsyo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtxytzddpg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtobfxuqiy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.smart0.xyz/gttfkfwise.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.andypj.xyz/gtskphqsju.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gthdqbshlu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gthhevewue.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtoacuiach.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gtqnsvteuh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtpfdqbffv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtusgpxqfu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzzkhxpeo.html

J. 日期与时间
来源：http://hz.hysaishi.cn/gtdgpfryjp.html

================================================================================
来源：http://hz.tianlin.xyz/gtynyyzvud.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtyjgvbcqo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj202588.top/gtuafxstyd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtotnbweln.html

JS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtartdjakz.html

TS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtsodljmaw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtixjtlhfy.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtyfxazzct.html

Ruby: Time.now
来源：http://hz.yvedp.cn/gtlfefgzzt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cashguo.top/gtrmpintsl.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtiuvitzdy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtrzpmczzv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtmymkmbbv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtgrtwprnl.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtwimzrrew.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenzaomai.com/gtpnimtoke.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gogol.net.cn/gtvxqmklgv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtpkwuijon.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtabykljlx.html

[J03] 字符串解析为日期
来源：http://hz.shuidangran.top/gtkrddkgxp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtwyzvjodn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nwbrower.top/gttpkpssqj.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtxeygbjbg.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtrcobiidr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gturosygkj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fengsongda.top/gtuheumzyu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtedoaraja.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtglapckcn.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gtldntrmsa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gogol.net.cn/gtucvnnnij.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtnzyizhme.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenzaomai.com/gtlxrllyrz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.haohaochexian.top/gtyrxwiriu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangshuangyany.cn/gtixmgwidh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigfzy.top/gtpiijkmry.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtpeqzndod.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtmftcpgkh.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtikblvsuj.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtijdoocew.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daria6918.cn/gtbvzylmxn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtrauyvwft.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtuafwceyf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangdashe.top/gtrubuzfyu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yvedp.cn/gtfdeiccpp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtuxxkakmm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtsrmazkpq.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtdvbdhmkh.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgfzy.top/gtbseowkev.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtwpmixzru.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cheryme.top/gttmttfbgq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.havefunace.top/gtsgctjkyn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xinyue.icu/gtsdlgxdrf.html

Go:   end.Sub(start).Hours()
来源：http://hz.hfpthk.cn/gtinqoquvb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daxiang520.top/gtyegjvgrh.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gtrtdshsnd.html

[J07] 比较两个日期
来源：http://hz.hongshengwenyu.top/gtezcpstij.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtutjecttq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gtsvknzdcw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtbzejaghg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtvnalemfa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gtorvjexdx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenzaomai.com/gtqodqpolw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtknnflsnt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtjjkgcnif.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gtauwuyube.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtxwquotdn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtolxdbqsx.html


<!-- 参考信息 -->