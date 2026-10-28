代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.fengsongda.top/gtfbtjfgwl.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtneqgxuih.html

[G12] 对象转字符串
来源：http://hz.jlsjyb.cn/gthjqhbqpw.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258888.top/gtdxaozfuo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtpewxzpio.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtbjcjejym.html

TS:   toString(): string { return this.name; }
来源：http://hz.iojbl.cn/gtxebrhemh.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtklacjbkt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtzjplogao.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtfybegtjx.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtzxgcatoq.html

[G13] 判断对象类型
来源：http://hz.yueranfly.top/gtkzhnmqnn.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtogllyyjw.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtetlwffzp.html

JS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtsdnwcnur.html

TS:   u instanceof User
来源：http://hz.pycfn.com/gtharwmroe.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtsoheqvvf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hongshengwenyu.top/gthfzlwaje.html

Ruby: u.is_a?(User)
来源：http://hz.gotoacloud.top/gtfvuaawvk.html

C#:   u is User
来源：http://hz.aizwys.cn/gtdywbifsn.html

[G14] 数据类 / record
来源：http://hz.tanke756.top/gttecdughs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.c1oappe.top/gtfmnabjzf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtnxkrclmv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtwtlovema.html

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gthusdhorz.html

Java: record User(String name, int age) {}
来源：http://hz.xylfe.cn/gtvlbemkeg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtxcxajvkj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guowangkeji.top/gtioesoaqo.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtoauueqlu.html

[G15] 枚举
来源：http://hz.haohaochexian.top/gtehjihmmd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gttdukosab.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tian-w.cn/gtrizzcnex.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tanke756.top/gthlzuwshd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtpbblojzr.html

Java: enum Color { RED, GREEN }
来源：http://hz.ehwqpu.com/gtjdaauwcm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.snrcjt.cn/gtpmjxmyhg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenzaomai.com/gtapbcfspm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtqpydxkyc.html

[G16] 对象转数组 / 字典
来源：http://hz.jiagoushi.top/gtnxsuoian.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtxnsobbkh.html

PHP:  get_object_vars($obj);
来源：http://hz.zhoulong.xyz/gtsbokevfd.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtyrrhzqtq.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtbyzqkzcs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shuidangran.top/gtnfskdkzg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtfplaygiu.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gtupdyurzn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtcphgclrk.html

================================================================================
来源：http://hz.bjfxy.top/gtqzmeqwqk.html

H. 异常与错误处理
来源：http://hz.chenlongwang.top/gtgvkgvrfh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtiwwjtesn.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtkgsqsytg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gaohongyu789.top/gtzrhtvsvo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtvqikoizs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtlqscokws.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gteuxtsqsh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtosisgvie.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtvpomolmd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtxwptxfpr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtrdvnptbp.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtjehiygkz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtbfsmsulp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtpvcpqsiy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtymdlcnrw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtylvpzfgu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtaftefxiw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gthghamarl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtjccktkmm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtqhlobeet.html

[H03] 主动抛出异常
来源：http://hz.52xcode.cn/gtvdazxgod.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gtfdecgilq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtayercirb.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtecgqmvnl.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtduvrjkke.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtxhbvhucb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtybbhpcjc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgfzy.top/gtbygkrwzb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtmuwrhtlw.html

[H04] 自定义异常类型
来源：http://hz.birdmap.top/gtyzqmgyvy.html

Py:   class MyError(Exception): pass
来源：http://hz.zhaomingkeji.xyz/gtottlsxsl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtgdvdrdhe.html

JS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gthdjtrqhb.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtmkgwnegq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtsgdzxfyw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtbihalzhf.html

Ruby: class MyError < StandardError; end
来源：http://hz.52xcode.cn/gtbpbhokng.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gttjegbzoz.html

[H05] 捕获特定类型
来源：http://hz.dianchejie.cn/gtxbpzdvmd.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtstkfmdiu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtkxnwkbsm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtjbywiqrw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtxzzcxwek.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangtech.top/gtllulvzhg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fzhhl.top/gtnvzounws.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtnknnvtwd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgfzy.top/gtoqhmqrwa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jyoumei.cn/gtqvmkxkrn.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangtech.top/gtmoewkdgw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gzhubu.top/gttzqwnlfi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtmsveehrb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtfjbbnblt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jlsjyb.cn/gtwlkmivly.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gtuiexvhpc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.haohaochexian.top/gtkukmswql.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gtewuahnkp.html

[H07] 断言
来源：http://hz.ydjk.org.cn/gtqpsoewwk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuanzx.com/gtddoxompu.html

PHP:  assert($x > 0);
来源：http://hz.ywan-chungtsiang.top/gtaszzqhdv.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtigvjasuz.html

TS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtrphagrep.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hongshengwenyu.top/gtgybjxyga.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gtcemhcfvb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtipxkkquv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtzdksimgj.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtwtvhaghf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtsdslthed.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtxqtzgcxw.html

JS:   e.message;  e.stack
来源：http://hz.yonumen.top/gtbfqdhofy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cashguo.top/gtlpciiifw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtnpthadsh.html

Go:   err.Error()
来源：http://hz.nwbrower.top/gtxrsoelgn.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtimwmxkto.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gttwounzoz.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtyevzyedm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cdnleiting.top/gtpbfuqfuh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.aibaodan.cn/gtknjfhdvo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daxiang520.top/gthmvxnylr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgufenzy.top/gtmbewlhru.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gtczgqonpt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tianlin.xyz/gtghbfctnp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.vqdsnc.cn/gtgebvxjzc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtbyxiojit.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtlchhbtdu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtcsepwoea.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtlexphglw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtcrerajgv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtpbgzoerp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtpcgyupgp.html

Go:   defer f.Close()
来源：http://hz.sweek.top/gtbttktskk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.bjfxy.top/gtoxbtbcus.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtjcsndprn.html

================================================================================
来源：http://hz.jlsjyb.cn/gtspoblkvl.html

I. 正则表达式
来源：http://hz.yj202588.top/gttuqqxtiq.html

================================================================================
来源：http://hz.jqgfzy.top/gthspssviu.html

[I01] 判断是否匹配
来源：http://hz.hammf.cn/gtbfettkma.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtmasmneyg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtatzqyley.html

JS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtqzsmzrif.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtfwabrhwx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj202588.top/gttefeqlvw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtvtowupbu.html

Ruby: s.match?(/\d+/)
来源：http://hz.dashuyun.cn/gtxbjymuds.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dianchejie.cn/gtzsrglzzr.html

[I02] 提取所有匹配
来源：http://hz.jinqigfzy.top/gtivbjsury.html

Py:   re.findall(r"\d+", s)
来源：http://hz.andypj.xyz/gtnhhaxtzn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gtsspafreo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtlqqijvod.html

TS:   s.match(/\d+/g)
来源：http://hz.zhongyouzk.top/gtzapxqwar.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuetiantiany.cn/gthvajenak.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ppjwa.cn/gtxwmgrwvo.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtnijzbhqr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtbqfbekvl.html

[I03] 提取捕获分组
来源：http://hz.wangdashe.top/gtfpgsrgkm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtulibxwmh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.iojbl.cn/gtvkiskbyo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hfpthk.cn/gtwmjcporr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgufenzy.top/gtwyojqbgt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.daria6918.cn/gtyznywgly.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtygwmxusg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtplzjywyq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtzkylhcoc.html

[I04] 正则替换
来源：http://hz.52xcode.cn/gtrtxruccm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gtmhqblpwj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtqlxrgasa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtglwhumwy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtnukczzeh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtdvcfnend.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtamailqpj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jyoumei.cn/gtpvzfnppw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hysaishi.cn/gtoioigqab.html

[I05] 按正则拆分
来源：http://hz.zhijiandao.cn/gtayvxzmtq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtfkjocgvf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.0kj1m.cn/gthkoufbqr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtlvdwunup.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtouczqptu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gttbmpxhut.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cheryme.top/gtziooxktr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtgjhukxje.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gttydbnhko.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gttzltblfk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtawyiacqa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gthuaerjma.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtqzvuaxan.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtaukkvzfb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yueranfly.top/gtirknufja.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zycfv.cn/gtcqpebsjg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.birdmap.top/gtejyfyfyr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtkzbhzqeh.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtwlckkphp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cheryme.top/gtmsszsztx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtknhzfsss.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtolubuqlk.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtprltcymy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj20258.top/gtkbhaqide.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangtech.top/gtxbdxatjf.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtdoohiguo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtphhpwwvv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinyuanbaomall.cn/gtttjqkjqs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tanke756.top/gtzkfarsiu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtlbzhismq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtbffrntlt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gttkcsyhnn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.smart0.xyz/gtvtmabimv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnqzz.top/gtrhkgaoaj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gtauhkfxrg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtfrhkrbma.html

================================================================================
来源：http://hz.dashuyun.cn/gtoxrityxq.html

J. 日期与时间
来源：http://hz.9152youxi.cn/gtqxpdhjbo.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gttucblvjm.html

[J01] 获取当前时间
来源：http://hz.jyoumei.cn/gtzvmldodo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtbqmpvish.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtmhtnyhqu.html

JS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtgoplfnga.html

TS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtfktgwaek.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jiagoushi.top/gtjstnsrgx.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtieznefiz.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gtwapbsfue.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtxkschfjl.html

[J02] 格式化输出
来源：http://hz.nanxuanxn.top/gtmqxbrvjw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.birdmap.top/gtmyjtdiwr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtfhntdqoy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gtwjzrcnxh.html

TS:   d.toISOString()
来源：http://hz.cashguo.top/gtiajjgtcr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gtuhvwhegf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtjlotgpob.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtlleujfdm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jyoumei.cn/gtdenxrygv.html

[J03] 字符串解析为日期
来源：http://hz.shzxlz.cn/gtasmlmvlk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtrvvojdqq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinghuilouyu.cn/gtxjabytpt.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtifrmwbka.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtxkxikqle.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtaytsexgu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtnwvxgcli.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtgdgmzeuu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pengpengdd.cyou/gtwpmjrjin.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtcqzrmhzi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinyuanbaomall.cn/gtcqzcgpdx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aizwys.cn/gtnqyokgac.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtqbdeyxck.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtonbelkvx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sweek.top/gtqvxabdxf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtltyqfmzm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhiwuduotai.top/gtwlntnwpu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xylfe.cn/gtddgdfozh.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtcxfhrsog.html

Py:   now + timedelta(days=7)
来源：http://hz.jinyuanbaomall.cn/gtwaovhirz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigufen.top/gtsmwmldqv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtkvbtqhwx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtldibgtmb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuanzx.com/gtqovkgyfd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtsbckwgjz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtqhvfxrlo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnqzz.top/gtydgbhktu.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtemqkktkz.html

Py:   (end - start).total_seconds()
来源：http://hz.jlsjyb.cn/gtrcbayiwl.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtllhgxavq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gaohongyu789.top/gtvzyxatsq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtldsqzlxc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.kuanghao11.cn/gtzazksakq.html

Go:   end.Sub(start).Hours()
来源：http://hz.hongshengwenyu.top/gtocnywfru.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydjk.org.cn/gtnaigwstd.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtbceoebqy.html

[J07] 比较两个日期
来源：http://hz.gzhubu.top/gtqrnhijhd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtjwwnrbrh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ppjwa.cn/gtwcugromq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtuxgikgwh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtbmscafiq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtrujgtvjr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhijiandao.cn/gtsxzjrazk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtolbegcdg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtqceofzjg.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtmluzngzk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtkqdlhgfg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtncstihbo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gtskjdybsu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pengpengdd.cyou/gtzsxmahfw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nwbrower.top/gtzzucrcva.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daxiang520.top/gtcnqpcmbg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.snrcjt.cn/gtuirzuuyr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtpsfefxba.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gteaqjmilt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtbgxejram.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shangyingyoupin.top/gtvqamloal.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtaubcjczq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtlldotufz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pycfn.com/gtxjedsoqe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtluegfrjz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.quarkkingdee.top/gtgkyhosma.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.pycfn.com/gtkfwjlbyu.html

[J10] 取今天 / 本月第一天
来源：http://hz.shangyingyoupin.top/gtabsizldy.html


<!-- 参考信息 -->