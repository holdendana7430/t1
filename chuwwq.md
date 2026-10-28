代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtzgbaovvp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gtuxikxgkc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cqqwz.cn/gtayyaqumi.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtwuiyfzjv.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gtvcyvowyu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtibdcrkyb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhengqikj.top/gtrttlktwk.html

C#:   interface IShape { double Area(); }
来源：http://hz.gotoacloud.top/gtztmouhpt.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtxvfcfryt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gaohongyu789.top/gtxhgzabzt.html

PHP:  public / protected / private
来源：http://hz.gaohongyu789.top/gtoonzdlxr.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtnflsbhmu.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtjabitkyy.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtpgkzqxug.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.meibo888.top/gteikomkjb.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtyrzuztak.html

C#:   public / protected / private / internal
来源：http://hz.zhoulong.xyz/gtmytmcpor.html

[G11] getter / setter
来源：http://hz.sysykeji.top/gtpxfteqmc.html

Py:   @property 与 @x.setter
来源：http://hz.ywan-chungtsiang.top/gtwmrzzekr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtwqynvgjp.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtvauznoto.html

TS:   get name(): string { return this._name; }
来源：http://hz.nwbrower.top/gtjhbaaika.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtyvouydae.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xinyue.icu/gtyzalkkpk.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtzjtaitbv.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtzufzcgbe.html

[G12] 对象转字符串
来源：http://hz.jqgfzy.top/gtxqbuwwcx.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gtlmykudbb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtdhzktnun.html

JS:   toString() { return this.name; }
来源：http://hz.zhoulong.xyz/gtjlnlaomx.html

TS:   toString(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtswfzncvw.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gtbklnmqyh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenlongwang.top/gthzzfwzbw.html

Ruby: def to_s; @name; end
来源：http://hz.snrcjt.cn/gtonqwadfq.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtcchijnfj.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtckqavsav.html

Py:   isinstance(u, User)
来源：http://hz.zhijiandao.cn/gtyrleuwme.html

PHP:  $u instanceof User
来源：http://hz.meibo888.top/gtgcgmtmoy.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtglvtisyn.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gtbvtkeiij.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gttfersldb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gtqedbkusz.html

Ruby: u.is_a?(User)
来源：http://hz.cucudq.cn/gthbycvewo.html

C#:   u is User
来源：http://hz.316326.xyz/gtsicbvzac.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtppjmjydq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtuwnmruwh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenzaomai.com/gtecmyibdg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daxiang520.top/gtsvilxdqa.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtaefpuavr.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gtofjmddgl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gtykhnvapa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtogojzyml.html

C#:   record User(string Name, int Age);
来源：http://hz.hammf.cn/gtdckbfjay.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtwybpvnht.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtzycdjhxv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtxocdxygb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtuetxyryt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtdxiymvvk.html

Java: enum Color { RED, GREEN }
来源：http://hz.feifeiyinyue.top/gtkppzksne.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtmjwoweuz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gtuwfyrmaz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtjzkrpgvw.html

[G16] 对象转数组 / 字典
来源：http://hz.gotoacloud.top/gtpbqaqrsh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gogol.net.cn/gtqckszsqr.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtjssklltl.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtnuxmjpxd.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtrpbnemkq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtwyiwbbck.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gtpsjjkupp.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gthdkaxtul.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtlyxcprmz.html

================================================================================
来源：http://hz.aizwys.cn/gtnyhjeqbe.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtvcxqobfn.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvdyhiyuh.html

[H01] try / catch 基础
来源：http://hz.yangfankeji.com/gtateofcun.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtoavvlhla.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gthtuaxegj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtkpmilpst.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtqxruyeos.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuanzhike.top/gtytrbpxwg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tian-w.cn/gtldbqagqx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtygirqhjr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xinyue.icu/gtsnwbpyfe.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtjlivkpua.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hfpthk.cn/gtgzcokoue.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtyebfnayo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtzkzhfehj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtsqcswjbh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtyeccoxpc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangshuangyany.cn/gthpwglmsc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jianghu66.top/gtjzhdbxiu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gttqbfxzzx.html

[H03] 主动抛出异常
来源：http://hz.kuanghao11.cn/gtwffjwcme.html

Py:   raise ValueError("错误信息")
来源：http://hz.quarkkingdee.top/gtyeqxbyus.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtgsfgozub.html

JS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtmjaehqws.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtudvtrrit.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtbnroyslj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gtmjmcoqmo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gogol.net.cn/gtwfpsmyfl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtowfiyxwp.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtcdnibcxp.html

Py:   class MyError(Exception): pass
来源：http://hz.wangshuangyany.cn/gtfezeepcs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtzoeiwrfn.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtgfilfzdh.html

TS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtsbuhxqmh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtahrshpte.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gthopoojls.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtrubgjsse.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtxqdlgvzg.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gtqekpnfwt.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtlasrzsty.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.feifeiyinyue.top/gtcxgxqyzv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gttqzxszxo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtbqnvqsig.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gtlgksebph.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gtcvszpmhd.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtlfxinpii.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtrltrjmku.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gotoacloud.top/gthaoobikn.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtgdsvnqtx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtepwnynmc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtkwhpaurz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtfpafsfka.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtitppqhai.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.vqdsnc.cn/gtjrtbduqg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtrjsrwqjc.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtrrfntntd.html

[H07] 断言
来源：http://hz.hnqzz.top/gtccxgzjjp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hongshengwenyu.top/gteanzmrgj.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtdlfxyhpl.html

JS:   console.assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gtkoavlrxq.html

TS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtilshsoev.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtrobmqvca.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.52xcode.cn/gtdmjxikwe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuetiantiany.cn/gtudizvdwa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtubwbrhlf.html

[H08] 获取错误信息与堆栈
来源：http://hz.xziqi.cn/gtkltkquwv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gttmupadpu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gttvoxojzt.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gtwzvgaouo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tianlin.xyz/gtpwxoujnk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtzvvniidf.html

Go:   err.Error()
来源：http://hz.smart0.xyz/gtshtixhdp.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtrgjwzuhv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.snrcjt.cn/gtmhzzowle.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtufzigoko.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gteseauhkp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtmqasrzcv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtuioczdio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhoulong.xyz/gtbcjzdljf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gthongultj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jianghu66.top/gtpknrmhdg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtrcjhtazk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtuszouxfo.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtjvsyomgf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gtofxkston.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gttklgczef.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gttclxumyz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtlptnkuxq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtfuawixun.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtjcxqekbn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cucudq.cn/gtfzglvkol.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhengqikj.top/gtlxrzsico.html

================================================================================
来源：http://hz.cqqwz.cn/gtcrqminia.html

I. 正则表达式
来源：http://hz.nwbrower.top/gtwkbdmpts.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtbuddrgto.html

[I01] 判断是否匹配
来源：http://hz.nanxinkj.top/gthqkwmcux.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhongyouzk.top/gtvbmftksk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtzfxqgwup.html

JS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtchgverku.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtyynjotzs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtvezhlads.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtuphmpkxj.html

Ruby: s.match?(/\d+/)
来源：http://hz.0kj1m.cn/gtakiicqcy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtykahxzfq.html

[I02] 提取所有匹配
来源：http://hz.smart0.xyz/gtxvoyirnk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtaibodmrw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtohxvtnvm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pengpengdd.cyou/gtohhhonmd.html

TS:   s.match(/\d+/g)
来源：http://hz.hongshengwenyu.top/gthyxvjjvs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangkeji.top/gtrstnsqqf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenlongwang.top/gtlezsznqc.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gtrqbrfvpz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yongpay.top/gttbaxjpuu.html

[I03] 提取捕获分组
来源：http://hz.xingfuxueyuan.xyz/gtdsxxqpof.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtfzlcsuov.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtmexezajc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtyhzegzpv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuxming.cn/gtdelrixty.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtdbourlpn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtmqbvadjw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gthheigmub.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtxneranbh.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtaxozlkcs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtpunbrfhr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtbcbryoaw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gthzgsmvrg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtxdyhglio.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.havefunace.top/gtdkrkoymk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtjhxikhhg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtfhnhqlne.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtynfxkovc.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtnaxvwldh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gteaooblxx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.feifeiyinyue.top/gtbckvaaxx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtrcmubnjo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtutvqxpvo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtxxodwwiw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtedgrdbiw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtvegaoohq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.havefunace.top/gtksmrpehu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtvnehbgsb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtbgduwkim.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gthlzpvjmw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtwswhyprf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtlqsumbwb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.vqdsnc.cn/gteulaxvcx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gtnzoudwcu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtkznithot.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtpkzafrcr.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinghuilouyu.cn/gtfyaqxuzc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtckzapkzx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtwkiauqjy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yonumen.top/gtodbfnzbw.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtndobzxbx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtowclxqvz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgfzy.top/gtbxsejqep.html

Ruby: s.scan(/error/i)
来源：http://hz.snrcjt.cn/gtsjmqwiww.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.kuanghao11.cn/gtoeteioyh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hywenlv.cn/gtgwmrlvzm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gtlksicrjv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gtezruunwq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtrmevfnls.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtcpvyzyxq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtjzuehrpe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gteehrphxz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtaipowrgi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtiovuruku.html

================================================================================
来源：http://hz.xinyue.icu/gtuiabjlkm.html

J. 日期与时间
来源：http://hz.sysykeji.top/gtwlbivrvm.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzxfwdxnd.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gtgaxaxdry.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtweemakzx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtrwqqhqax.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtwsdcgifc.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtwlgmubrt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ywan-chungtsiang.top/gtprsrstha.html

Go:   time.Now()
来源：http://hz.ppjwa.cn/gtuzlhvjdg.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtmocwrwpr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnxiangtu.top/gtbcajlrdz.html

[J02] 格式化输出
来源：http://hz.jyoumei.cn/gtkbomjtqv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gterjqaoan.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gttvnuodzz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuetiantiany.cn/gthgjfutxg.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtqknavrsh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gtxkmthxgk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tianlin.xyz/gtrnhzlfis.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtvqlcoeqo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gthikpfppn.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gthjjvmzan.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtgbwididv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jlsjyb.cn/gtjcnhoibw.html

JS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtqtqohspj.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtauqxpdjw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtcfylrdgn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gtfkxvlcma.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtrpndcxiq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtucmdaxqm.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gttgrezfzi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.feifeiyinyue.top/gttqijalxz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtpxkpnigl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jiagoushi.top/gtutrlwlll.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yueranfly.top/gtwjswxaos.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.quarkkingdee.top/gtxbxyryqz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuanzhike.top/gtkzglzfgu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hfpthk.cn/gtkfqthdpq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtwsckdenq.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinghuilouyu.cn/gtzpkctpfg.html

Py:   now + timedelta(days=7)
来源：http://hz.yongpay.top/gtxkmdwsrp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtxhfbdnjs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtbybmgiwm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtkijwaysy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zycfv.cn/gtgqeyxvev.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gthxvdnkoh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtxueptayg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtaksrgolb.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtbbmibuiw.html

Py:   (end - start).total_seconds()
来源：http://hz.zhiwuduotai.top/gtqvkbxuxy.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigfzy.top/gthkimbvmx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gthjngxwhi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hysaishi.cn/gtaqyidkro.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhiwuduotai.top/gtiuvbuxzz.html

Go:   end.Sub(start).Hours()
来源：http://hz.hongshengwenyu.top/gtotvnprgl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtjzmmqmio.html

C#:   (end - start).TotalSeconds
来源：http://hz.nwbrower.top/gtvfrlcfwu.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtahjxtxna.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtlplfdens.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhaomingkeji.xyz/gtfunugzoy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtihectbqy.html


<!-- 参考信息 -->