代发 wailian999

[G10] 访问控制
来源：http://hz.9152youxi.cn/gteqmdbdjj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pycfn.com/gtshbplzgs.html

PHP:  public / protected / private
来源：http://hz.jlsjyb.cn/gtxkryimso.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gtwpagnqao.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gtdxtufdjl.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtqxntfqnn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtyecjzfuq.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtoygyycra.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gtwebmgdot.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtxkemweit.html

Py:   @property 与 @x.setter
来源：http://hz.gaohongyu789.top/gtkuzoanyw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj202588.top/gttbbnwqvv.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gtkoqkbtka.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtocxnkghl.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtldfdhtfq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtijlydjpm.html

Ruby: attr_accessor :name
来源：http://hz.zhijiandao.cn/gtnraagosn.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtgdepicdc.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtcjdzqeap.html

Py:   def __str__(self): return self.name
来源：http://hz.cdnleiting.top/gtpzovctpn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtgaqcocld.html

JS:   toString() { return this.name; }
来源：http://hz.9152youxi.cn/gtfwbjytki.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtapzsiqvp.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gtzwlpkzdg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtsupmvzfa.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangtech.top/gtdzthvjbm.html

C#:   public override string ToString() => Name;
来源：http://hz.daria6918.cn/gtbiyuijga.html

[G13] 判断对象类型
来源：http://hz.gotoacloud.top/gthczpezhd.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtjylnxaip.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtdjnmmlsl.html

JS:   u instanceof User
来源：http://hz.xinyue.icu/gtbjxivrrv.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtwnkxcdyl.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtpxylvclq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ehwqpu.com/gthvjbcnde.html

Ruby: u.is_a?(User)
来源：http://hz.9152youxi.cn/gtgrtookgr.html

C#:   u is User
来源：http://hz.iojbl.cn/gtjtswrkoz.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtgazlpmkm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shzxlz.cn/gtkcqlfabk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtkgekqgwo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tianlin.xyz/gtikwakplb.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhoulong.xyz/gtfbegjgkk.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gterjnzcxn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtyjwhhelw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtsvljgshv.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtklaotddl.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtfbfbysmb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cashguo.top/gteywqlscr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gttkenbbih.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtwiukmzif.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtnhvtvhkw.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtizqbcwpg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gttgbgkqbv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtefxekrcy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtxxxlasio.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtozttmcil.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gtwwuodroe.html

PHP:  get_object_vars($obj);
来源：http://hz.gaohongyu789.top/gtpnzkqcpw.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtqqfkszzm.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gttuypdfcq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhengqikj.top/gtqbddlrjz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtqwqvmcvo.html

Ruby: obj.instance_variables
来源：http://hz.ivvv.top/gtqdqsekbi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtznzimalo.html

================================================================================
来源：http://hz.316326.xyz/gtynwyqdvi.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtppaqbnva.html

================================================================================
来源：http://hz.yueranfly.top/gtexoipwfz.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtcszdpxau.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sxryk.cn/gtzqxuxzuy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtvbhziemc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtseqjxxye.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gtmexjaxge.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenjidiqi.icu/gtkptruiqw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ywan-chungtsiang.top/gtrfynbpdq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ivvv.top/gtduvvsgbu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cheryme.top/gtczsnkutd.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtdbloxeoo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dianchejie.cn/gtlqphwxgv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gthwkgnszm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtmkgkrjzu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtjpmzasbn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtthdsphcy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tianlin.xyz/gtrgijmtkv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtbaljfzql.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yonumen.top/gtoyazkdnk.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gtzngpzctk.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtqsxfjdwp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtrrmfpfuk.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtmmgixber.html

TS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtnrlvdvwg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtxivhlyis.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gtnabmhfnu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daria6918.cn/gtcagdepxn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtrvfaakqi.html

[H04] 自定义异常类型
来源：http://hz.nanxuanxn.top/gtkjqdwscp.html

Py:   class MyError(Exception): pass
来源：http://hz.mhx1999.top/gtlkiibfnw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nwbrower.top/gtxwaioqeb.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtjqwnxuqc.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtxlgorgaa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gththxejsq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtwkwkbfge.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtskwqmgup.html

C#:   class MyException : Exception {}
来源：http://hz.hnqzz.top/gtdtosaztc.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtgbcajube.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtrcbjeiwl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gzhubu.top/gtslhhhzuv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtnilkixhv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtyfhymaxb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.havefunace.top/gtzukbjpoj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuxming.cn/gtnbdoftyi.html

Ruby: rescue ArgumentError => e
来源：http://hz.sufxvd.cn/gtovsraxuh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhengqikj.top/gtxaxjordc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hongshengwenyu.top/gtmznhzexl.html

Py:   value = d.get("k") or default
来源：http://hz.gzhubu.top/gtwqbprmlp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zdqjudy.top/gtbgqzrfiw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtkcnmwflu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gteosptpcp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtjofirjvo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtaldvhryy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gtiejfzjgs.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtallwssom.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gthquftpuz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hywenlv.cn/gttqshaugr.html

PHP:  assert($x > 0);
来源：http://hz.tian-w.cn/gtavcasckk.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtjcyrrwbq.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtbagldgad.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gtaimmynkb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.haohaochexian.top/gtiucnfvug.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtxetfgnqa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258.top/gtyswsfwyc.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtjooxalzd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sufxvd.cn/gtvvhjutbk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gtdumpfiid.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangkeji.top/gtupqpzoqr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xinyue.icu/gteoosrvkv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gtumpcuegs.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtwizisxuk.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gttiypibyx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yanxiufei.cn/gtcsolrfed.html

[H09] 带错误码的异常
来源：http://hz.jqgufenzy.top/gtnuqueryo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtyvnugzhk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtdvqgwufo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shzxlz.cn/gtlteqpuiu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtksnbrqsz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtcyrecdka.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gtxvevtylb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.andypj.xyz/gthozuacko.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxinkj.top/gtvrcjtwze.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtpjqqtzna.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxuanxn.top/gtfqfxbkpx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtzejjtyfl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtnjxyigty.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtkfpcakvl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtzkurplyz.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtmymdvaxg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gzhubu.top/gtbdsttncl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtjulijyho.html

================================================================================
来源：http://hz.yj202588.top/gtxaupqgeq.html

I. 正则表达式
来源：http://hz.ivvv.top/gtwtgrmuxt.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtpnosgqpc.html

[I01] 判断是否匹配
来源：http://hz.ivvv.top/gtsngvpwyc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gtaxwdeqpf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhongyouzk.top/gteapoyxup.html

JS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtqqludgot.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtdahdwyok.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnqzz.top/gtlzqhtwop.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gtiqasfupr.html

Ruby: s.match?(/\d+/)
来源：http://hz.fzhhl.top/gtcpphvxic.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gtmwmmvmsy.html

[I02] 提取所有匹配
来源：http://hz.svipenyu.cn/gtmcvbmlwe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cucudq.cn/gtwnccclyf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtjwgcgpry.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yongpay.top/gtmxcwgncc.html

TS:   s.match(/\d+/g)
来源：http://hz.hfpthk.cn/gtjbpecbwl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtamsydicb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgufenzy.top/gtkvqxdtev.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gtlsndklsh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.9152youxi.cn/gtxpztwuzp.html

[I03] 提取捕获分组
来源：http://hz.wangdashe.top/gtvwynlwcu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zdqjudy.top/gtzihalmjx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtqjkalrhs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hongshengwenyu.top/gtnkjkfaro.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gthuxyatqj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sufxvd.cn/gtkrgshsis.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.iojbl.cn/gterwmcnqb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtumczylby.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yvedp.cn/gtsdnjgtmc.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtuuybumth.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aizwys.cn/gtqxlnjowu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gtdixkacir.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtnnyyoybh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtubsikuet.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtmmemfqua.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtbnycrgbs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtptynmlsy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.andypj.xyz/gtrajqulsu.html

[I05] 按正则拆分
来源：http://hz.zhengqikj.top/gtrlefuxuu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtilhtsdry.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhaomingkeji.xyz/gtzhsqjlqa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtoygclcqg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtpncyhbqa.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jyoumei.cn/gtmdarkxla.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gtvzbcvbdr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtkfeleukr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shuidangran.top/gtnasyhllr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtvoxzllpm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gttgsoksso.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtwhrdmkpq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtnzonurcv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtaeplsqpr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sysykeji.top/gthweblmeg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pengpengdd.cyou/gtpnucbcnu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuetiantiany.cn/gtxsprhuzd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtxvvvxvbt.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtogjhlcdr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtlbfggzum.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtzbrcxycc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shuidangran.top/gtpixpomss.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtdpstylel.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cheryme.top/gtudwilgzh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tanke756.top/gtewusmxho.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtpccqdiim.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtuekzuftg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnqzz.top/gtieeqcdih.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258888.top/gtukzwllvm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtapmnrjsn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtcvvsakmh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtzklwzdth.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gthkwxjekv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtvdzwxujp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gtbftvddmn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtgwesescm.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtuxxowasl.html

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gtlugfjvox.html

================================================================================
来源：http://hz.jiagoushi.top/gtfcdhvfcx.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtabxlozzj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtjlyosfod.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtgwrmauec.html

JS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtgxyhceot.html

TS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtdjyrbcxq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtwpednxzx.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gtlhgjxity.html

Ruby: Time.now
来源：http://hz.gogol.net.cn/gtftojwjrh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgfzy.top/gtghbjghzp.html

[J02] 格式化输出
来源：http://hz.yongpay.top/gtfietttbs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtwjqaocrh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtshprfttu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhoulong.xyz/gtpdakusav.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtykoczvzo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guowangkeji.top/gtjztsxyhf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gtqugbqkcl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtntxzooqk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.316326.xyz/gtdvseyzvl.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtcvqdrihp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtfthbuedl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtudfrzrot.html

JS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtotpnghmy.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtliltnzws.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtjltwyerg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aizwys.cn/gtakrjurqw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gthvgvapge.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guannengcc.top/gthgaozbiq.html

[J04] 时间戳与日期互转
来源：http://hz.aizwys.cn/gtdsgkptfc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtnoqjacfa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gtjopahbyf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sufxvd.cn/gtusrpsrbp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.iojbl.cn/gteseicwai.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtyzliodyo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtxzvyjyeb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gtqfzefpqn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtsraqjrun.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtnqqfafjc.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gtvhsozsro.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jiagoushi.top/gtixoxtnoa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtxguwfnsj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gttidqdgia.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fengsongda.top/gtdojdhrwl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtlnzudmga.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtuvcddwxy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ywan-chungtsiang.top/gtdhulvxpn.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gttkcbjhoi.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtehryntty.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtjlwvsuem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtqdquswvx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhixingplan.top/gtumwkldtl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258.top/gtgpuuvaop.html

Go:   end.Sub(start).Hours()
来源：http://hz.ivvv.top/gtjelrjjoh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sxryk.cn/gtrjjpuwms.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtmbgwkcmd.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtfahuygpy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtvwvzgqyy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shuidangran.top/gtyicgnzpd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtirojscpp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtsxndeuzu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtkhrxrpek.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtrnsopgiv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtotqbbmfs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtosyeeolu.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtkuitziai.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtqjvnppwu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daria6918.cn/gtiwqgwstj.html


<!-- 参考信息 -->