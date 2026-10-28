代发 wailian999

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtnlwmtznw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gtkphszzok.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtnzuzcput.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtgnqhyamz.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gttztuxewf.html

Java: public / protected / private / 默认包级
来源：http://hz.hammf.cn/gtjnmoyekt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shangyingyoupin.top/gtnhpdsuul.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtfvthxmpq.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtjkgifspc.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtteoccmpl.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtheugiphl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtidwfdwtn.html

JS:   get name() { return this._name; }
来源：http://hz.ppjwa.cn/gtadndguvu.html

TS:   get name(): string { return this._name; }
来源：http://hz.svipenyu.cn/gtwmwggsdc.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gtsqquowen.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtzwayhuss.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gtmqpkwtqa.html

C#:   public string Name { get; set; }
来源：http://hz.yvedp.cn/gticbuvpnu.html

[G12] 对象转字符串
来源：http://hz.zhengqikj.top/gtoavlvucb.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtnvzptwix.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtnldlnvug.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtquqntxnh.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtwogaozgq.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtqarduyrg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtagogwjbu.html

Ruby: def to_s; @name; end
来源：http://hz.nanxuanxn.top/gtfwboxdks.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtnlwtitkp.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtbfxeoiax.html

Py:   isinstance(u, User)
来源：http://hz.svipenyu.cn/gtelciqrok.html

PHP:  $u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtpyzpjgpz.html

JS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtzeqonlzw.html

TS:   u instanceof User
来源：http://hz.yongpay.top/gtcdspxwom.html

Java: u instanceof User
来源：http://hz.chenlongwang.top/gtxrqtlrtl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yongpay.top/gtiyrlsmux.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtnnmraldh.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtziakezzf.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtpqyrlxhk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgfzy.top/gttgkycuxq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hongshengwenyu.top/gtdduwcumw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zdqjudy.top/gtghstcglp.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtbfepdzpz.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtjlgwtzak.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daxiang520.top/gtyljrujsq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtqzsadyhm.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtlhbatdlt.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtheirnhxi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenjidiqi.icu/gtpclchpyj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenjidiqi.icu/gtllynpaym.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ybcxt.top/gtmooeryke.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtipydejrr.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtvjiqnabk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangshuangyany.cn/gthtwviijz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.52xcode.cn/gtfmyhudcc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtpbspxmtl.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtvcmtylqt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtwyxhwkxw.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gtmswurmyx.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtmqdxmqpe.html

TS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtlyomvglp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtbiimdrjv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gtnqzvqtsb.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtiyayaofx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtcxkiuygr.html

================================================================================
来源：http://hz.hnxiangtu.top/gtynsldjsg.html

H. 异常与错误处理
来源：http://hz.quarkkingdee.top/gtjultwbty.html

================================================================================
来源：http://hz.xuanzx.com/gtdqqjsdhf.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gttjudeida.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtdusqacmp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtqupcphfq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gtekvjylvk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtzmzytodt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtsjqzmkxo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenlongwang.top/gtsugotbpd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gtklanpjqp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sxryk.cn/gtujyrtgfc.html

[H02] finally / ensure 收尾
来源：http://hz.daxiang520.top/gtyawxzbhw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fzhhl.top/gtsygopgyo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtbuwcltwz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtwsdwnomq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtyleewzqf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtkfsqkstf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xylfe.cn/gtfilgtlvb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gtvvhauvhg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtmldpoooq.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gthcferlhp.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gtrfyaqdre.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtrebgjhlw.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtgkcbnadt.html

TS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtqxfpgjjh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtwetiwizo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtqolofril.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtffvbdgsx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtdzpogwbn.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gthqqiwmdy.html

Py:   class MyError(Exception): pass
来源：http://hz.wangshuangyany.cn/gtbwsqxpdw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gthqvkmfty.html

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtiwpsrhll.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtekilhbnm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtdzjlmatr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtywgsuczn.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtqpwrpbno.html

C#:   class MyException : Exception {}
来源：http://hz.iojbl.cn/gtbrzybbhf.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtvvestyqe.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtyrpgugpj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gtrckzruof.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtqscrcbqp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtzfovpdsx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tian-w.cn/gtmtvnlrsh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtqbfkgtmh.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigufen.top/gtwzjyfifi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.9152youxi.cn/gtdszykadj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.quarkkingdee.top/gtfbnyjcvu.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtsisbkkzw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtzntlvcwi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhongyouzk.top/gtiditpomj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtmlvenivq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtbpzpspvr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gtychvxcat.html

Ruby: d&.dig(:a, :b)
来源：http://hz.iojbl.cn/gtbzqjobej.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtoagwwbtf.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtkuxiqsen.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtfyetgskf.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtiyqbgkpx.html

JS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtvxxlwsyd.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtjbknqgdi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinghuilouyu.cn/gtbsewrmfm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtcsycgrdm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zdqjudy.top/gtqkpbxkqb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gthmhmtqmv.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gtvaciklfe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gttjuursir.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtujveoabg.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtqfffldat.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtyuwrbfve.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fengsongda.top/gtuepktvsm.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtsmcqkikl.html

Ruby: e.message;  e.backtrace
来源：http://hz.guowangkeji.top/gthcjirhrj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnxiangtu.top/gtwedjtsqh.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtcvklgvnt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.mhx1999.top/gtlsxsdmsf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhoulong.xyz/gtlbucuzfi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258.top/gtfzdgbvqu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtbotvkdnz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yueranfly.top/gtvnltauwe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gtqkdsehyg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinyuanbaomall.cn/gtrjrjqkdo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtvkedgjha.html

[H10] 资源自动释放
来源：http://hz.chenlongwang.top/gtpycbrmev.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gtdtqbsyrf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtdpmuppja.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gttszcqcxf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtifqyipyz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhiwuduotai.top/gtbwgbgqwu.html

Go:   defer f.Close()
来源：http://hz.tianlin.xyz/gtmtbhfcaf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gtjetjnuex.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnxiangtu.top/gtpqippzvk.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzsnwtkku.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gtxjczfvul.html

================================================================================
来源：http://hz.redwolf501.top/gtstlagqxk.html

[I01] 判断是否匹配
来源：http://hz.cashguo.top/gtamqesqko.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtyjilelik.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.redwolf501.top/gtsxcblnnd.html

JS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtdsifoqev.html

TS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtlwtbtito.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtgghmxrit.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtirrldclp.html

Ruby: s.match?(/\d+/)
来源：http://hz.jyoumei.cn/gthpqnsivf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtxjkildgw.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtafnocjck.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtzzhuusvc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgufenzy.top/gtiwsdbkne.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dashuyun.cn/gtfejmmtlw.html

TS:   s.match(/\d+/g)
来源：http://hz.chenjidiqi.icu/gtrjwsbgxd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guowangkeji.top/gtyhxavbfr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.havefunace.top/gtfjqkothe.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhengqikj.top/gtbcipfuki.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhijiandao.cn/gtdbszxzad.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gthgrkovcu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtdwtkcbny.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtpuehglin.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fengsongda.top/gtwvqyurqy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtibtioqtw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtzzbudyul.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtmcclcbyn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtdoqajxtb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtylzqbfhh.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gttpamuobd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ehwqpu.com/gtqflnqion.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gaohongyu789.top/gtwzbvvgha.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtexrvpbhw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtrkuhsdty.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.feifeiyinyue.top/gtxwxdkorf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shzxlz.cn/gtjdycodxn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtkeoccpey.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gtkxvyxmhk.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtjzdkmhre.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtnnedawwx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aizwys.cn/gtjdnhuzox.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtqmdmbtsf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtszrblhli.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxuanxn.top/gtcwpexqch.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtvklykzjx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtckdtthey.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pengpengdd.cyou/gtpfifaixc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtjnvgmcdf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gthvsmgtbm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtqestxgav.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtkfewzyul.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtffoxdqqk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gtfnvfpmru.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gtkbymxkco.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.quarkkingdee.top/gtpsosfssl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gteurfwklq.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtplozlisx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gzhubu.top/gtvsapmyrs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtbiyhqzdc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gthipmlssu.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtlkhjiaou.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhaomingkeji.xyz/gtazocvxbm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtrpfeqdpv.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gteprydbio.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtxfjrxlym.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtvxwsczss.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtcvwjjtzk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tian-w.cn/gtlegibonr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtjfhuvqml.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtehfkcptq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtgjwbyogi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtnxfoujee.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtsinyqhcc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtuzetypor.html

================================================================================
来源：http://hz.sufxvd.cn/gteispbxjl.html

J. 日期与时间
来源：http://hz.chenlongwang.top/gtpzslrwpv.html

================================================================================
来源：http://hz.ybcxt.top/gtsmwtmtym.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtyggocrfn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fengsongda.top/gtojxbtnvv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtmilikdtd.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtiahafxsf.html

TS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtjdptdcus.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gtoesjjoqi.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtkrwzyaxi.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtqgjbwdqd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gtdapvolsw.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gtiebzyold.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtemiamgbi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtfqcdfgic.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.0kj1m.cn/gtxnotqezx.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtzjcibfng.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gtydhtnnzo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuetiantiany.cn/gtdgnxmwuk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtmkwvhmbq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jlsjyb.cn/gtbjrclynv.html

[J03] 字符串解析为日期
来源：http://hz.chenlongwang.top/gtuurgnkwz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydzc1.top/gtziochphs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtwinururt.html

JS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtttsrauvj.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtdtgvfbtf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtgzvpqtwd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.birdmap.top/gtauxtgbxl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtdzpjumto.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtzwiatvyb.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtjovitkaa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pycfn.com/gtnpwiuvol.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gtfzkjpewx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.redwolf501.top/gtimvgdzcb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangtech.top/gtyfxlfdxe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj202588.top/gtfgcrybzw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gtxhcnbyxn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gttapivxzj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yvedp.cn/gtiqqaaixn.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtuipueeud.html

Py:   now + timedelta(days=7)
来源：http://hz.zhijiandao.cn/gtbzroevht.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.redwolf501.top/gthztyyapi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtpkwlwftb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtcmlxwwfv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtywjeuwah.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtraemkzvw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hywenlv.cn/gtgpkihlej.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtmrgwsmla.html

[J06] 计算两时间之差
来源：http://hz.ppjwa.cn/gtwajeemyk.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxuanxn.top/gtltjpszpt.html

PHP:  $end->diff($start)->days;
来源：http://hz.jyoumei.cn/gtrbqgicaj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtsygrnhti.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtyrqsmoly.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.bjfxy.top/gtatcckytj.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gthlvgdzim.html

Ruby: end - start                 # 返回秒数
来源：http://hz.kuanghao11.cn/gtxdxgvuba.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtrrbofpmt.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtordonafg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtskxspqnt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtdzmgsggh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtbkazxfhq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtzclxnurk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtpqisvcum.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.mhx1999.top/gtshrdfdhq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtcojfeexd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtglokdzeh.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gtbtvubmvo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigufen.top/gtucfghpuz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shangyingyoupin.top/gtzannzuud.html


<!-- 参考信息 -->