代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gtwdrbzaoq.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtswjizdsh.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gthtqpdcpy.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangkeji.top/gtjkuudevv.html

JS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtgbzfvnrq.html

TS:   super.greet();
来源：http://hz.yuxming.cn/gtdmlvefvl.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gthylijfrr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtrrujqmui.html

Ruby: super
来源：http://hz.daxiang520.top/gtnzsixirv.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtckpyalku.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtvmdbqqrg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtkmuzjafs.html

PHP:  public static function f() {}
来源：http://hz.hywenlv.cn/gtxukutwbd.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtqamgbyyj.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtnjkihtaa.html

Java: static void f() {}
来源：http://hz.gaohongyu789.top/gtznjwvlwu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtpjkxjduw.html

Ruby: def self.f; end
来源：http://hz.cqqwz.cn/gtrrasfegn.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtxocfiswu.html

[G09] 接口 / 抽象类
来源：http://hz.dashuyun.cn/gtznlrlvpt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtifxnvzmb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dashuyun.cn/gtuuvehoqs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.mhx1999.top/gtasxrexid.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtbbylnlye.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gtawpiboop.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gtbmhbodmk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtmwbsirye.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangkeji.top/gtmaqdkoxd.html

[G10] 访问控制
来源：http://hz.xuanzx.com/gtczsbdwjd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigufen.top/gtfgtudcxf.html

PHP:  public / protected / private
来源：http://hz.ydzc1.top/gtamemlfnh.html

JS:   #private 字段；其余公开
来源：http://hz.0kj1m.cn/gtywlpswht.html

TS:   public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtmqevmnzm.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtvtldiokn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258888.top/gtiyjtkwnc.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtpgiljcss.html

C#:   public / protected / private / internal
来源：http://hz.guannengcc.top/gtmuvwjgds.html

[G11] getter / setter
来源：http://hz.jinqigfzy.top/gtfjkgfxwm.html

Py:   @property 与 @x.setter
来源：http://hz.hongshengwenyu.top/gtwixrjyiv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtpjimjoqh.html

JS:   get name() { return this._name; }
来源：http://hz.hywenlv.cn/gttuegecmv.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtmrkmuuph.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gtbqfxceda.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtrxbsipww.html

Ruby: attr_accessor :name
来源：http://hz.birdmap.top/gthrtmjedq.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtyeiicsiu.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtudpcwipt.html

Py:   def __str__(self): return self.name
来源：http://hz.zhoulong.xyz/gtfmcfaswp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtjszedeot.html

JS:   toString() { return this.name; }
来源：http://hz.ydzc1.top/gtbvfrviyb.html

TS:   toString(): string { return this.name; }
来源：http://hz.xinyue.icu/gtwiseohje.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxinkj.top/gtvowbczzg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gtcsyjjmux.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigfzy.top/gtsicmkojo.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtmdkfnqvf.html

[G13] 判断对象类型
来源：http://hz.cashguo.top/gtrdxordcl.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gtqvcdonot.html

PHP:  $u instanceof User
来源：http://hz.yongpay.top/gtgyrdkstf.html

JS:   u instanceof User
来源：http://hz.zhixingplan.top/gthrvwfsth.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtofivzrca.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gtcmjalcfc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gthvfqegrv.html

Ruby: u.is_a?(User)
来源：http://hz.yj202588.top/gtuhrjzkpg.html

C#:   u is User
来源：http://hz.hammf.cn/gtubejpubi.html

[G14] 数据类 / record
来源：http://hz.jqgfzy.top/gtcmfzxbiu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daria6918.cn/gtioduedlr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tian-w.cn/gtkgyrpmrw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtmkrdgpir.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangtech.top/gtyisbvtdn.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gtnnvibhqw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zycfv.cn/gtwtopfxuc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtoqkmmuvc.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtvfodyfmh.html

[G15] 枚举
来源：http://hz.gzhubu.top/gteipuwrrf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pengpengdd.cyou/gtqawlyfwn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gtlmkslrcg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cucudq.cn/gtzkimchln.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtpjlrxxzt.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gtruvjfxqu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hywenlv.cn/gtnfhwecle.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtlkjkgebz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtamyohafj.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtutjmxxre.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.snrcjt.cn/gtenzofrpz.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtwtqbuiqh.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtruxcspaz.html

TS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gttkebueta.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtibazemoh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guowangkeji.top/gthhewcebg.html

Ruby: obj.instance_variables
来源：http://hz.birdmap.top/gtdkmsobes.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jlsjyb.cn/gtlywuihhk.html

================================================================================
来源：http://hz.yj20258.top/gtludupbny.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtvnknpwgv.html

================================================================================
来源：http://hz.haohaochexian.top/gtptdgcjbr.html

[H01] try / catch 基础
来源：http://hz.jiagoushi.top/gtmsdailct.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhiwuduotai.top/gtxbwguszj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gttjenmini.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtapcxhyzg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtjbtfbvkk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gthrvcdick.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtcmysofsh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ivvv.top/gtigimzgpz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shangyingyoupin.top/gtjivqiout.html

[H02] finally / ensure 收尾
来源：http://hz.xylfe.cn/gtfuhgjjow.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuxming.cn/gtdyimgxzl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtztnowaqx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtlkufavpf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtsupsfrrf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gteiaglcjg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtvizpgiee.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtnzcsxepy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.52xcode.cn/gtkkvyvtce.html

[H03] 主动抛出异常
来源：http://hz.52xcode.cn/gtzebsztug.html

Py:   raise ValueError("错误信息")
来源：http://hz.xziqi.cn/gttjdjrrps.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtrgayubsi.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtwpkycfhr.html

TS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtkalwhzgb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtrdwnfbxu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gteyjgeocr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ivvv.top/gtlooryunw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtlqldihsk.html

[H04] 自定义异常类型
来源：http://hz.zhixingplan.top/gtbglmxtcw.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtbijfqiym.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cucudq.cn/gtkftuzjzd.html

JS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtnanaiifq.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtbqewycql.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yvedp.cn/gtkzvbzyfj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtuoodhkrm.html

Ruby: class MyError < StandardError; end
来源：http://hz.tianlin.xyz/gtnkrsfggw.html

C#:   class MyException : Exception {}
来源：http://hz.hysaishi.cn/gtrtsvekuh.html

[H05] 捕获特定类型
来源：http://hz.daxiang520.top/gtmamfbidc.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtumewjcph.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtthzjndvb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtgwdrdtxd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtbzvpenbk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtrymafsuo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtnoqkfwne.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtqgvrbodp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtrxcbnixi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtmtfumqtn.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtaklmjngs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtfhjycufz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtoojikpfw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtdhlomtqs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtdmzhqnlo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtvlusjqch.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxinkj.top/gtikojkugn.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigufen.top/gtrmgvimtx.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtibfpcoww.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtkcyvupkc.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtnjxaypnh.html

JS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtmgekjetw.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtryyajjil.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yongpay.top/gtyyfopytr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fzhhl.top/gtjldwmmys.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gtpittnlbw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtvxmzmsgt.html

[H08] 获取错误信息与堆栈
来源：http://hz.shzxlz.cn/gteeizkydm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhixingplan.top/gtsxnjkjdi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgufenzy.top/gtrdxnbdob.html

JS:   e.message;  e.stack
来源：http://hz.ybcxt.top/gtorhazlnz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtvdddyjgg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.andypj.xyz/gtezqxxhga.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtxmswtwun.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtoiyykilm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgufenzy.top/gtmgjpewtp.html

[H09] 带错误码的异常
来源：http://hz.tanke756.top/gtczhajbln.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtfuhavcqd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtybjkkxfc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnxiangtu.top/gtulrdvvzq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydjk.org.cn/gtvswmxyqm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtzymjinpu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258888.top/gtkfkfjass.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gtmvxowytk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtysngpuum.html

[H10] 资源自动释放
来源：http://hz.havefunace.top/gtkgbycmcw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gthuhmvewh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtuzffnnri.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtnvgcuykw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtsdonvqwt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yongpay.top/gtvmatzvwz.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtlxnjbtxy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fengsongda.top/gtsryzthvv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gtcqbolmpm.html

================================================================================
来源：http://hz.chenzaomai.com/gtmmjbjywa.html

I. 正则表达式
来源：http://hz.ppjwa.cn/gtyocagfve.html

================================================================================
来源：http://hz.zhixingplan.top/gtdnmiawma.html

[I01] 判断是否匹配
来源：http://hz.dashuyun.cn/gtnfwuwzml.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtrsszfokf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtmvdhvosf.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtaofbzics.html

TS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtasjofsxx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.kuanghao11.cn/gtxjvuewlc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tian-w.cn/gtvhdujojy.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtbcojvwcs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtmcgcakqq.html

[I02] 提取所有匹配
来源：http://hz.jinghuilouyu.cn/gtjcqaliwc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shuidangran.top/gtrihkrrui.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtfsdetkuy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.svipenyu.cn/gtkmvugoix.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtmwwozssx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtnojrdhqq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xinyue.icu/gtjmbtiaok.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtgmimdoxc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gthybwvfwq.html

[I03] 提取捕获分组
来源：http://hz.wangshuangyany.cn/gtkuxepnem.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtsfotyisw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtrnvfoebx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtgzalbqes.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtkmcxxdwq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gtpcnuqeoo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gthkmtflai.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gtrismfnsx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gtrwtyaupo.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtuxadsoty.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guowangkeji.top/gtapmjhbfn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtkejlmova.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtqhsniiot.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtshrqjjje.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhiwuduotai.top/gtbwpwiytj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtdfvqsjro.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.bjfxy.top/gtihjmtxjo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gtfauarvqn.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtcifhwxvu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ehwqpu.com/gthxbagxqx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtfojsjejd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtumineywt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtnbovkcsq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gtnywjickz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gtfyzqzyxm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtailqojfk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxinkj.top/gtujgscmgu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydzc1.top/gtsbdhyayd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtnwjfektt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuanzhike.top/gteepcgshg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtwvxcvqso.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtbbshtnfw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtroporkun.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtvpwqgntr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtpydovhwn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtjpkyvnhs.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtvxwwdfoc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtixuxeqat.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtrunrynlp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aibaodan.cn/gtqmotegax.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gttupfuyzt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtoxxftyan.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gthwhqxgkn.html

Ruby: s.scan(/error/i)
来源：http://hz.snrcjt.cn/gtdmwqsgau.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gtmjczfmmo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtqvrdxoks.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hongshengwenyu.top/gtpfamelba.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gthybrebow.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtloyicont.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtfeobfwjj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydzc1.top/gtdiobnvam.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtkycliute.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangdashe.top/gtycokrptm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtuuqfqmos.html

================================================================================
来源：http://hz.guannengcc.top/gtwwmlkgon.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtqmrtrqek.html

================================================================================
来源：http://hz.zhixingplan.top/gtojcnqmoj.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtkryfktqa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtexyhdkdc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gttqltqguu.html

JS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtiqrqmkvf.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtxqinssqx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtgeudhboo.html

Go:   time.Now()
来源：http://hz.zhengqikj.top/gtgxpyowdd.html

Ruby: Time.now
来源：http://hz.zhoulong.xyz/gtopjgfgbe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cashguo.top/gtjuoxbljd.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtqihdfeyr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtuluxscjj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtwkfyzvch.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtdvhfbncl.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gthurtotfr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtqkgcptpi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ivvv.top/gtrddjrcgi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtkrrmcnrc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shangyingyoupin.top/gtoripphci.html

[J03] 字符串解析为日期
来源：http://hz.52xcode.cn/gtjzreiies.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.svipenyu.cn/gtyhqxuogm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtiydhpnaf.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtwsxrxser.html

TS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtewwquseq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtsjwjmngj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtbywrxjjl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtlggpbhdg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gttrerjkrm.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtmvwtdkma.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtjlmrmstk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shuidangran.top/gtgbydhksm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtenjhauxa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sxryk.cn/gtrqacxabm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gtenllhvyp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtcytehitl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangtech.top/gttxpznkof.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.svipenyu.cn/gtrlyrfwtq.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtjwkjdhzw.html

Py:   now + timedelta(days=7)
来源：http://hz.yangfankeji.com/gtlwclfsss.html


<!-- 参考信息 -->