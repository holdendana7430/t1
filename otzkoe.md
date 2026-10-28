代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtkfcisljg.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtpyywwhyb.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtabrhidhb.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtezdagmuj.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtflhlwvvm.html

TS:   super.greet();
来源：http://hz.0kj1m.cn/gtnngihreh.html

Java: super.greet();
来源：http://hz.havefunace.top/gteemthody.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ppjwa.cn/gtlkcvumvk.html

Ruby: super
来源：http://hz.daxiang520.top/gtetnhgyzs.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtwqifncjo.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtprurrzab.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.bjfxy.top/gtheqssymd.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtqyykjpdf.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtavkuzdwg.html

TS:   static f(): void {}
来源：http://hz.xingfuxueyuan.xyz/gtyrpihvsv.html

Java: static void f() {}
来源：http://hz.nanxinkj.top/gtjgdotdxl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hongshengwenyu.top/gtfneghrni.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangtech.top/gtgkkgnuwe.html

C#:   public static void F() {}
来源：http://hz.cucudq.cn/gtzqfstcct.html

[G09] 接口 / 抽象类
来源：http://hz.yonumen.top/gtqtgewiwj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtuwxvencl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cashguo.top/gtcslbpqig.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtohntngkp.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtmepthupi.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gttuxkmhji.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtnilgcuzg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangtech.top/gtbnccqhug.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtupchrbke.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtcozrqgqg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtbycopqje.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtjeyirrru.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtqwhaxyve.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtkuerghoj.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangkeji.top/gtfjsvdmdz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtokhxuqmh.html

Ruby: public / protected / private
来源：http://hz.jyoumei.cn/gtgghzvwbo.html

C#:   public / protected / private / internal
来源：http://hz.shuidangran.top/gtyapttkbv.html

[G11] getter / setter
来源：http://hz.0kj1m.cn/gtasbjqkdm.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gtcqvrbdpn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ybcxt.top/gthxvqwzhf.html

JS:   get name() { return this._name; }
来源：http://hz.guannengcc.top/gtzlbynonf.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gttypxerwd.html

Java: public String getName() { return name; }
来源：http://hz.pengpengdd.cyou/gtmhshthnv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gturgwghpk.html

Ruby: attr_accessor :name
来源：http://hz.smart0.xyz/gtgqxfcbvi.html

C#:   public string Name { get; set; }
来源：http://hz.xingfuxueyuan.xyz/gtnomooqlf.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtvkujzhfh.html

Py:   def __str__(self): return self.name
来源：http://hz.aizwys.cn/gtjzjibvre.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtskieapzp.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtbrkjjojq.html

TS:   toString(): string { return this.name; }
来源：http://hz.yueranfly.top/gtnrbvefqh.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgfzy.top/gtheimbrkn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.haohaochexian.top/gtuiccxumt.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtrvepbqed.html

C#:   public override string ToString() => Name;
来源：http://hz.pycfn.com/gteaazlyhv.html

[G13] 判断对象类型
来源：http://hz.vqdsnc.cn/gtqwufknoh.html

Py:   isinstance(u, User)
来源：http://hz.iojbl.cn/gtoeiowiuo.html

PHP:  $u instanceof User
来源：http://hz.sysykeji.top/gtthvelpoa.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtadunuwtg.html

TS:   u instanceof User
来源：http://hz.jianghu66.top/gttdsgqzlx.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtritrigxz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigfzy.top/gtluebfrii.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtejyqooxv.html

C#:   u is User
来源：http://hz.xinyue.icu/gtrijcaoiy.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gtcfazifcq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtrlwevpll.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hongshengwenyu.top/gtmkcvoeto.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtxlbbchai.html

TS:   type User = { name: string; age: number };
来源：http://hz.sufxvd.cn/gtcsnvhjsm.html

Java: record User(String name, int age) {}
来源：http://hz.vqdsnc.cn/gtgrycffft.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cashguo.top/gttnzgwdkt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtleaicqsz.html

C#:   record User(string Name, int Age);
来源：http://hz.chenzaomai.com/gtnpfkklhd.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtnmaenhgl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sweek.top/gtxkyxjtui.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtgxdooqiu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtyulesxpt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtdidufjwi.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtbnchbckp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtunpxtisg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtsgcbrrrr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtzwzzaopx.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtgrgyazsb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tian-w.cn/gtlplqpykv.html

PHP:  get_object_vars($obj);
来源：http://hz.yangfankeji.com/gtxulolfuy.html

JS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtuxezyziq.html

TS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtmdetestn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtoebpgbhl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtdmcxmzel.html

Ruby: obj.instance_variables
来源：http://hz.xuanzx.com/gtsfngyowe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtqltddxmm.html

================================================================================
来源：http://hz.yangfankeji.com/gtllpsklqn.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtblzahgbl.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpyzsnoik.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtyejyfjgn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtlsmgilky.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtwuagagph.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtineyoufh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gtieszrexg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtilblgkxe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shangyingyoupin.top/gtasruklcx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtdhucdzdr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtcumhtipo.html

[H02] finally / ensure 收尾
来源：http://hz.fengsongda.top/gtogkqugdt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtsjihwcrg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtxokzbwbb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtgzoexsjb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtqlmggmlf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtuquzykec.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhengqikj.top/gtvcugnceg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gtoswtkehl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhoulong.xyz/gtamzcbsxj.html

[H03] 主动抛出异常
来源：http://hz.yj202588.top/gtiazmvhur.html

Py:   raise ValueError("错误信息")
来源：http://hz.gotoacloud.top/gtkzihgrbm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtcshsfuod.html

JS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtjjmonjjm.html

TS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gttckztxfc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtirutxpba.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtngquvmzs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhaomingkeji.xyz/gthsshhtvq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtuwlnuutq.html

[H04] 自定义异常类型
来源：http://hz.hongshengwenyu.top/gtofkcusee.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtgctunsfh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtmagpislq.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtyoaubtro.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtgkfyqmpk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gthuqvmfiz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtkjcplmgv.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhongyouzk.top/gtrjewmprx.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtxqeihwnc.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtyqmabcae.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gteeqblvtr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtybtkcfgm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtaahnsgxb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtlzjctlkd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gotoacloud.top/gttawocaql.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gtqndeurpc.html

Ruby: rescue ArgumentError => e
来源：http://hz.aibaodan.cn/gthyaqyzxh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtbnpokvba.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtojjudjlv.html

Py:   value = d.get("k") or default
来源：http://hz.zhoulong.xyz/gtkbwgnwul.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtbyasidwb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtwmythuhc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtvrscgqao.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangkeji.top/gtawikkdem.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj202588.top/gtkpdolpct.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guannengcc.top/gtohrxizpe.html

C#:   obj?.A?.B ?? default
来源：http://hz.ybcxt.top/gthmfbdlsv.html

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gtmtkzikke.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtwztekrtq.html

PHP:  assert($x > 0);
来源：http://hz.haohaochexian.top/gteulflyey.html

JS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtpzmdfzef.html

TS:   console.assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gteuqotttn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuxming.cn/gtubbgaayy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.9152youxi.cn/gtxqihcfnd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.c1oappe.top/gtvhzcorom.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtcbwkmngv.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtcfurspzz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtqoqqqlsu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtjwucbdbm.html

JS:   e.message;  e.stack
来源：http://hz.fengsongda.top/gtutenjaug.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtgtblvwag.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtsfdrlhnf.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtpggaseht.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhijiandao.cn/gtgoayrets.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtauugqleg.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtbdhlnnmv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtnwhoqkgr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhixingplan.top/gtpfamzugk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yonumen.top/gtejkikiqr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtuhkngmfz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gttcoesptg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtzguvuesj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtsgsjatwg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gtiarxljak.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gtkujpquvh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sweek.top/gtbbchilmp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jyoumei.cn/gtximecbog.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtkzwadcoi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtctfpgtad.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gthcfddpzd.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtugqazzgd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtrzmdizew.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtquqmtyqa.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthbjubqid.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtwmmwqugm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbyfswhwq.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gthholcyoa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtopzgdork.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtbxpabdcp.html

JS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtwblxwupo.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtuwzhrbca.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhiwuduotai.top/gtqhhmnfib.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sufxvd.cn/gtaifsgfjh.html

Ruby: s.match?(/\d+/)
来源：http://hz.9152youxi.cn/gtmidpvagk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtffyuqlqp.html

[I02] 提取所有匹配
来源：http://hz.haohaochexian.top/gtnznywhel.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtuitiybgk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gteigxlkwo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtxphhphew.html

TS:   s.match(/\d+/g)
来源：http://hz.xuanzx.com/gtsaszoqhb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtbewtlhvk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuanzhike.top/gtslofpyzq.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtmpuuhkkv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtytdwyvos.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtqxbqjwvk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtwzqzzeit.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtfqipglzh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gotoacloud.top/gtwecljpvq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuxming.cn/gthvbnehvw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtcucnltpo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtuvtrhsyc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gaohongyu789.top/gtupsmngpl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ivvv.top/gtqaosmzlt.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtdinprmmx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hywenlv.cn/gttcfqkkgx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gaohongyu789.top/gteafimmbb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtbhazgsmh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtqeldsclo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.snrcjt.cn/gtgdtkzgvr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hongshengwenyu.top/gtfzbwmqze.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sweek.top/gtrhkhqdox.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yonumen.top/gtrewjfrvu.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtgpdsuxzu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gthlynxvcr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuanzhike.top/gtzjpivyqk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gttmkovxgy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtrnzhnkxd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tianlin.xyz/gtkzcgmvdf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxuanxn.top/gtxgdnsyqx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gticpbwham.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xingfuxueyuan.xyz/gtadivgpqq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gtwjxjoqsn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtgvzdmbbe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.mhx1999.top/gtevrdnqcs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtnryvirlw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtiaelmwkv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ehwqpu.com/gtaqorwygt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinghuilouyu.cn/gtuugcaswy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtqlppkbof.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtsqdbkncl.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtifynjvwr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtdmotybyh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.mhx1999.top/gtmpuxzdmp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.birdmap.top/gtgxpsbaoa.html

TS:   /error/gim
来源：http://hz.sweek.top/gtqtvcwrvd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hywenlv.cn/gtsojrqisr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtkcjfwfis.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtnvrhwpgt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gtsrgdnunv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuetiantiany.cn/gtvbqcnlis.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhengqikj.top/gtxhffzqzk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gaohongyu789.top/gtnfznsvfc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtedzqgsot.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtojgpfwwo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtdxaesdwt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtsgltlrnk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gtskpwcdjg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sysykeji.top/gtkwifaclp.html

================================================================================
来源：http://hz.xziqi.cn/gtnsexswtk.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gteuqdibvq.html

================================================================================
来源：http://hz.sweek.top/gteiqbpucj.html

[J01] 获取当前时间
来源：http://hz.jianghu66.top/gtbbfuqsrj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtykvoqgjw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gthmxlccal.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtbokqzcqc.html

TS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtxnzhqgsr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtidpfowbt.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gttyhcutuj.html

Ruby: Time.now
来源：http://hz.jiagoushi.top/gtivpwtezy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhaomingkeji.xyz/gtnvmaozua.html

[J02] 格式化输出
来源：http://hz.jianghu66.top/gtgpsdaykj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtgtpregwi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtymvoabjs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.52xcode.cn/gtujvyvuka.html

TS:   d.toISOString()
来源：http://hz.jqgfzy.top/gtgnlomwdk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangdashe.top/gtftpiexpx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gtzyyuvurd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtocrkmrab.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuanzx.com/gtollstiki.html

[J03] 字符串解析为日期
来源：http://hz.iojbl.cn/gtozozzeiq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtomlvrpri.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtluyhswzi.html

JS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtvvxpkuki.html

TS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gttyvekkbf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtjksontsv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gtpxbnugus.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtalbqtlhk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gaohongyu789.top/gtrqrhqafm.html

[J04] 时间戳与日期互转
来源：http://hz.gogol.net.cn/gtuasfsmeg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gtfykilshj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtgnumaqrc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.c1oappe.top/gttkogeqjl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hysaishi.cn/gtnlykfykd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gthxbefjxr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gttbcwhzoy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtpqsviast.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtteakzqrc.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtjjesfrqv.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtjvocjtrg.html


<!-- 参考信息 -->