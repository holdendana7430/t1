代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.hongshengwenyu.top/gtojkwevze.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtugbfbwvi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hammf.cn/gttyivfvmx.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhengqikj.top/gtiaicnruj.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtadomrclo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhijiandao.cn/gttjimufbe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtnhutshsm.html

C#:   interface IShape { double Area(); }
来源：http://hz.316326.xyz/gtxqjwzkve.html

[G10] 访问控制
来源：http://hz.hfpthk.cn/gtduuajsue.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtbizzxvlz.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtpcntyyvd.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtyqjlgvwf.html

TS:   public / protected / private
来源：http://hz.mhx1999.top/gthwjldevy.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtgxmechvk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cdnleiting.top/gtyrwewnpt.html

Ruby: public / protected / private
来源：http://hz.wangdashe.top/gtefywnual.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gtpjgkeqfc.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtjqcdouth.html

Py:   @property 与 @x.setter
来源：http://hz.chenzaomai.com/gtgvdyhyas.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtllranjbs.html

JS:   get name() { return this._name; }
来源：http://hz.xziqi.cn/gtyvxyzesq.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigfzy.top/gtbsryhyoz.html

Java: public String getName() { return name; }
来源：http://hz.cqqwz.cn/gtepnyjmqv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtrsoqfabz.html

Ruby: attr_accessor :name
来源：http://hz.ybcxt.top/gtmnltfxlz.html

C#:   public string Name { get; set; }
来源：http://hz.ydzc1.top/gtdebirhco.html

[G12] 对象转字符串
来源：http://hz.jqgfzy.top/gtpawsrayp.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gtaxltwjqh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtbozwvuhe.html

JS:   toString() { return this.name; }
来源：http://hz.zdqjudy.top/gtvqjdevff.html

TS:   toString(): string { return this.name; }
来源：http://hz.shuidangran.top/gtozlcofyo.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtnqizrdwk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtyhscevwh.html

Ruby: def to_s; @name; end
来源：http://hz.feifeiyinyue.top/gtxzrnpacy.html

C#:   public override string ToString() => Name;
来源：http://hz.xuetiantiany.cn/gtzapyjbzl.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtnillhzsr.html

Py:   isinstance(u, User)
来源：http://hz.fengsongda.top/gtqhbbhhsj.html

PHP:  $u instanceof User
来源：http://hz.xylfe.cn/gtcijplbbw.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtgljxgbvo.html

TS:   u instanceof User
来源：http://hz.yuanzhike.top/gtdzxznqfg.html

Java: u instanceof User
来源：http://hz.birdmap.top/gtamfugony.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gttvqqmrno.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtholrmmna.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtekljrwem.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtqfezoopp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxuanxn.top/gtjiianquf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gtbtfvzhxz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yonumen.top/gtccpbqukl.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhaomingkeji.xyz/gtghxlbxpd.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtxjyhfrms.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtmqcqjcmg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gturgiysna.html

C#:   record User(string Name, int Age);
来源：http://hz.ybcxt.top/gtfgsfxhck.html

[G15] 枚举
来源：http://hz.chenzaomai.com/gtihhnontp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtovlakuvs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pycfn.com/gtwxutvrse.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtgcvroqto.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtfloqijou.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtzzkcnjmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtthddlllr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtjzhdgwet.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtplaxqpdu.html

[G16] 对象转数组 / 字典
来源：http://hz.zdqjudy.top/gtuzflmhmt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cheryme.top/gtzzbedjjh.html

PHP:  get_object_vars($obj);
来源：http://hz.sweek.top/gtpqsgjuqq.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtqjnzpnhu.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtrlftcwmv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtpntresvn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gtmvqmlknz.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtokyfxoes.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtspwqfuqo.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtzyiocmmp.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtjipcncpi.html

================================================================================
来源：http://hz.yuxming.cn/gtsgcpgodl.html

[H01] try / catch 基础
来源：http://hz.andypj.xyz/gtexktjeyw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtckjeccbm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtzwesdckf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtivvucxgh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gtsrfujynf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sweek.top/gtdswtnheb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenlongwang.top/gtewczzzai.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jianghu66.top/gtbloslaxz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gtlxjxbgee.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtzgdfuvrl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gtcipgevdc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtxntvucxo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtuqohgtua.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtrusumndu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtqcvkwxkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtialbsuoa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtpaubkffv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtrxmqjfvn.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtxtbqmqep.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangdashe.top/gtntgvtxaw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sweek.top/gtqtahxzlc.html

JS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtgpdivtyw.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtqcoxodsy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtpmnkixso.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yonumen.top/gtjrxoztnr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtndtbkpns.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.birdmap.top/gtevqjolmk.html

[H04] 自定义异常类型
来源：http://hz.hongshengwenyu.top/gthgysdfvz.html

Py:   class MyError(Exception): pass
来源：http://hz.shuidangran.top/gtqalalzik.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtjehlooyj.html

JS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtcdiziknw.html

TS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtovctqrre.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtmntppekv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hywenlv.cn/gtgvdeahwl.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtzpqcqyyq.html

C#:   class MyException : Exception {}
来源：http://hz.jiagoushi.top/gticvgsyhc.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtrjomomtp.html

Py:   except ValueError as e:
来源：http://hz.zhongyouzk.top/gtuiktexyw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xingfuxueyuan.xyz/gtikcpgpbb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtovfixhbl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtexwtbdnu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.iojbl.cn/gtqvuuoxxr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtzyvfoadj.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtdcxhmhpv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gthjniwjyi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtrvsldnjy.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtkqsmuzpp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tanke756.top/gtzlfryqtt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtzuhztvjt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtnumpfzqi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fzhhl.top/gtkvpccrwq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cashguo.top/gtdfjjkolf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pengpengdd.cyou/gtshuvjvax.html

C#:   obj?.A?.B ?? default
来源：http://hz.dashuyun.cn/gtpgthyxsr.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtbnnfasci.html

Py:   assert x > 0, "必须为正"
来源：http://hz.kuanghao11.cn/gtwjgbdibn.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtbddbrust.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtdpkrpnrw.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtwidgicpr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gzhubu.top/gthsnqqjnr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuanzx.com/gthdeuyuts.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtgszaqzus.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnxiangtu.top/gtvxujlraa.html

[H08] 获取错误信息与堆栈
来源：http://hz.guowangkeji.top/gtftwputws.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtqftlpdkh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtvmsxtahm.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtghxvikho.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj202588.top/gttfoiypru.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gtpysuqndg.html

Go:   err.Error()
来源：http://hz.pengpengdd.cyou/gtfbwmsyhu.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangkeji.top/gtkxzmjebl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.9152youxi.cn/gtnxporipm.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtkntgpwdg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gthwkbrvqz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.kuanghao11.cn/gtmzhxifqh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yonumen.top/gteocmqmvn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dianchejie.cn/gtyhngwyzy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gttlgxkdkf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtiykegttq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtxyhkquoi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258888.top/gtfgjrkkux.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gtqbxkryfl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtgjvhuubz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtokoicsod.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtkokfdctq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtkaxlvxlk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jiagoushi.top/gtssautscf.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtywhsvncn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daria6918.cn/gtghsexuvr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangtech.top/gtdvficrhm.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfrckbgkx.html

I. 正则表达式
来源：http://hz.daxiang520.top/gtnyjyyuzg.html

================================================================================
来源：http://hz.dashuyun.cn/gtqyjrnvun.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtwqwoyzeb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigufen.top/gtmsrfijvo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtoyckctwo.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtnulbdkwa.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtldukopny.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shzxlz.cn/gtbafdbkde.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gtlvhzbpoe.html

Ruby: s.match?(/\d+/)
来源：http://hz.fzhhl.top/gtihbisnxg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtntaatclf.html

[I02] 提取所有匹配
来源：http://hz.yvedp.cn/gtlodwwspi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gthfvwegxm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtmmqgfwbj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dianchejie.cn/gtjsvxdcbt.html

TS:   s.match(/\d+/g)
来源：http://hz.sufxvd.cn/gtjeewbkhy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtgvukivfx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nwbrower.top/gtzllphjnd.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtxxpzwqre.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gtulfrvcwa.html

[I03] 提取捕获分组
来源：http://hz.gaohongyu789.top/gtmcpakooj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtarxcfxxl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guannengcc.top/gtvxtnaudc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtxqbgcrln.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuanzx.com/gtegftdkgs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinyuanbaomall.cn/gtdtphtzdx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinghuilouyu.cn/gthfodygxf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtdbnvymsp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtugnwkhzk.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtantbzbni.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtdlsbowmx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtvabtnwxt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gttgdbshlx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtbidaqosw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gtnphlsblj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtupdchump.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtvmfpmdqr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gtldqxszms.html

[I05] 按正则拆分
来源：http://hz.chenzaomai.com/gtftpcirmz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtoiwjpxhp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtqosuxetz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtuwwmnaxj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtjxrfhboy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cqqwz.cn/gtzjuuinkb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xziqi.cn/gtkxsqpqnx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtpynjekwb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtbmlpnbwf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cheryme.top/gtvfbbvydu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtiavysiwn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gtxxxektlq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtnkaatsvu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gthmwzeiyx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtpfagiubo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guowangkeji.top/gtgunuzpyk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhengqikj.top/gtpwahjoma.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtlaztbvcs.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtddrmgsze.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gteqfnalnd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gtywucrmkq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtsgrpqgeg.html

TS:   /error/gim
来源：http://hz.gzhubu.top/gttuvgzsjr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhoulong.xyz/gttfafvkyf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.snrcjt.cn/gtmmicnpyr.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gtprmortua.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtfrjwxbiz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.redwolf501.top/gtvgtspssg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtulwziyoc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtancbxjes.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtuzhxnxso.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtzhrqmcik.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtvanwhdxw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gttigyxshf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuanzx.com/gtxlreuxmd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gttqxagjil.html

================================================================================
来源：http://hz.0kj1m.cn/gtxwajwumx.html

J. 日期与时间
来源：http://hz.cashguo.top/gthjphsobx.html

================================================================================
来源：http://hz.nanxinkj.top/gtqeegghlh.html

[J01] 获取当前时间
来源：http://hz.jiagoushi.top/gtazbxwqbh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtiyiurcmg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtryluphrp.html

JS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtcmlehmqb.html

TS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtmcwpyhxu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtrvyjemmi.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtsonzctjx.html

Ruby: Time.now
来源：http://hz.zhaomingkeji.xyz/gtemnmbevu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtydtmajhs.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gtjqpkbkes.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtjtqfrzcx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtlgtbzjgg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.0kj1m.cn/gtibpnhvye.html

TS:   d.toISOString()
来源：http://hz.xziqi.cn/gtcdcqeszh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtghyjqggg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtemothgzg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtmdqauged.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shzxlz.cn/gtfpinzudo.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtnrwvmeli.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtqixewgwl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gthhaoqray.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtrdptxiht.html

TS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtsumdxfzl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gtssdnppwg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yonumen.top/gtdjfzhdkb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtwdzthkon.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtizppjcqr.html

[J04] 时间戳与日期互转
来源：http://hz.ehwqpu.com/gtqcxvoctu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgfzy.top/gtggwowjim.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtujxftxdq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.mhx1999.top/gtprssfjwd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtupzerbei.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sweek.top/gtykbuyglz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhiwuduotai.top/gtzptfdayu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtbyoesick.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtsajopseq.html

[J05] 时间加减（加 7 天）
来源：http://hz.cqqwz.cn/gtejikfpca.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtsjafnros.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sxryk.cn/gtflugjlmo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtgofjtdvj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtftzrzsur.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenzaomai.com/gttgmljuko.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tian-w.cn/gtbxvmfzzi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtubgndyzf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gotoacloud.top/gtbylxijbn.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtrqtoactm.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtyrgmgfds.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtphsyqhjh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.haohaochexian.top/gtxqwykwif.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtpozdwnxg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shzxlz.cn/gtyroqshio.html

Go:   end.Sub(start).Hours()
来源：http://hz.yvedp.cn/gtutupqowr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtutajekui.html

C#:   (end - start).TotalSeconds
来源：http://hz.shangyingyoupin.top/gtmsjyyicg.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtuloyckzh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gthdmxujsz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtcbdivhmb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtspzkspgu.html


<!-- 参考信息 -->