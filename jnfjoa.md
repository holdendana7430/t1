代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtzrtkzupq.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhongyouzk.top/gttzinsysm.html

Java: public String getName() { return name; }
来源：http://hz.yuanzhike.top/gtlkbzhkfk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtoxzhaemy.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gtcolyhsum.html

C#:   public string Name { get; set; }
来源：http://hz.ivvv.top/gtkykmqbro.html

[G12] 对象转字符串
来源：http://hz.mhx1999.top/gtglzvjlqd.html

Py:   def __str__(self): return self.name
来源：http://hz.smart0.xyz/gtyovkttyc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtbqjrijnn.html

JS:   toString() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtfiqdiyfg.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtmbattqrs.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtbvocbhwd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtcmryyzpv.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gtwaopcxzx.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtkqauairz.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gththkdozc.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gticesukxs.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtmupsiwaz.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gtwbmfmbea.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtsimmrfeo.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtigzybrfz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hammf.cn/gtldhlmypn.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gttiinwrtg.html

C#:   u is User
来源：http://hz.aibaodan.cn/gthyvkztqo.html

[G14] 数据类 / record
来源：http://hz.jinqigfzy.top/gtnajhtftq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtbkhmnust.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtpzthqhxu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtzdpuizjt.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtqchekfvh.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtijwgmnnc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cheryme.top/gtnmqpluwa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shuidangran.top/gtbzdmjvdl.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtmmcrnydo.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gthqqjjlnu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtxzjgevfd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hongshengwenyu.top/gtjvhddvqe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.birdmap.top/gtqefeivyr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtoqkvkmos.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtgucfooeo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hysaishi.cn/gtihtrdlwr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuanzx.com/gtpbeomynf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtngtbhgxh.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtfckikzkt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtmaaykihk.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtnqftjmmr.html

JS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtqqnielsd.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gthcgecaxq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gtqrwcunmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtjoedxhps.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtscxtqerd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtyswwfhkt.html

================================================================================
来源：http://hz.zhixingplan.top/gtphjmuvni.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gttzgfhtbf.html

================================================================================
来源：http://hz.zhixingplan.top/gtkthhdeqb.html

[H01] try / catch 基础
来源：http://hz.hysaishi.cn/gtzpeunfqc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.andypj.xyz/gtbbhgemcn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gtnmniurqg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtcffmoumb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtobnsfmpz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.redwolf501.top/gtbcdrqmdn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.snrcjt.cn/gtdepnnigx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.redwolf501.top/gtngzllvbx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hywenlv.cn/gtgjhhzmwt.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtahznanza.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtnmrwjqsu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtcmqtexpr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtdbqpnozj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtidnlehut.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtrwzkiuez.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.vqdsnc.cn/gtgqzodjrm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtcigtcidv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtrbnjmdaq.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtcpxhoori.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtpgwjsmie.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cashguo.top/gtjomhypzy.html

JS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtrkevtpxc.html

TS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtbitkyqto.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtyvuxhfcn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daxiang520.top/gtghadftvd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtfvgviiqe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtomzmncfb.html

[H04] 自定义异常类型
来源：http://hz.jyoumei.cn/gtttsahouc.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtvlhmmexi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.andypj.xyz/gtsdffhsep.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtbykhehsc.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtcgkrwsht.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sxryk.cn/gtrlhkvxto.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sysykeji.top/gtjjfxzqic.html

Ruby: class MyError < StandardError; end
来源：http://hz.aizwys.cn/gtkvplaoiv.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtaezjlwdk.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtngafiqek.html

Py:   except ValueError as e:
来源：http://hz.yanxiufei.cn/gtywlvwjvu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gtbqgdkvlx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtrxtmupou.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtcnagghno.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtljpewbkd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xingfuxueyuan.xyz/gtlbjikuvi.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigfzy.top/gtmsomnvvh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtkzsahjvl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hywenlv.cn/gtldtobxma.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigfzy.top/gtavkqmjjf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.9152youxi.cn/gtluqxbgop.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtwdrvbjfw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtodsqogib.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gtvzfbvref.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtojgecuei.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pycfn.com/gtxscrijdn.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtzqtdhpll.html

[H07] 断言
来源：http://hz.guannengcc.top/gtsxbqzaoc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cheryme.top/gtceiylykt.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gtxclnsnmx.html

JS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtwmrlprjp.html

TS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtoljrzscr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xylfe.cn/gtdhdfesuv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhiwuduotai.top/gtutlompnm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sufxvd.cn/gtrsaliiul.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gaohongyu789.top/gtbmquvmbn.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtcbzzhtcu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenjidiqi.icu/gtgnfcixqo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtjfszypmg.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gtdbhacfzc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtrsdrviwm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtbspbiegu.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtnzogceya.html

Ruby: e.message;  e.backtrace
来源：http://hz.guowangkeji.top/gtsqzhdkth.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtybvzadok.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtcegblpqg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gtpfzzlbeg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gtrkzpdkaw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shzxlz.cn/gtxlqywfpx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258888.top/gtjyjduuaa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtvvgwfcfy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gteaydocdo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhiwuduotai.top/gtdiwpnomj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtpsjynyub.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gtewmohfwm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gtxbxcnmyy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtpddqehhj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtevpxwdxb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtepanmavt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtlhlccgvk.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtkobdyhaq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tianlin.xyz/gtxfzcityq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gturyyqngm.html

================================================================================
来源：http://hz.zhengqikj.top/gtlcrbxibi.html

I. 正则表达式
来源：http://hz.pengpengdd.cyou/gtuwpvtbma.html

================================================================================
来源：http://hz.yuxming.cn/gtylkypwvq.html

[I01] 判断是否匹配
来源：http://hz.hfpthk.cn/gtiuqxqook.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.c1oappe.top/gtwkcuhsda.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj202588.top/gttyqhalzh.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtbomdwfxc.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtirugsfli.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.9152youxi.cn/gthegoxhnv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fzhhl.top/gttxfbjvhn.html

Ruby: s.match?(/\d+/)
来源：http://hz.cqqwz.cn/gtzpqwjlti.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtyoykikkx.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtlugtnpax.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cqqwz.cn/gtejpcciko.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hongshengwenyu.top/gtrrivjkav.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtmfholpfc.html

TS:   s.match(/\d+/g)
来源：http://hz.zhiwuduotai.top/gtugzpdsxo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtupiddumf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtjimhpggz.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtoinsabrl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gtzmbydbxj.html

[I03] 提取捕获分组
来源：http://hz.sxryk.cn/gtehicakwv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtpeebzbwm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtqythasew.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtgwpuyoru.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtgauzpitp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinghuilouyu.cn/gtftclcdlt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gzhubu.top/gtlkjvqeng.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuetiantiany.cn/gtrsttohsy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtzeeclsrn.html

[I04] 正则替换
来源：http://hz.cashguo.top/gtilcgsicz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtweastens.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtdhnrazdv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtznsrcegg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtpadhpgdj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gthmofvuba.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.redwolf501.top/gtilipdtuu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gthpzrvyzf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtairrjuyw.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtitbbykrc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtzpvqcclp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtgucalerx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtchklgkcm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtkfkdwewb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtexnzdthh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.iojbl.cn/gtfttryetc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtrrvqghua.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fengsongda.top/gtgnsuaawa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cucudq.cn/gtneptpsau.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtllpwanyh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenlongwang.top/gtxypuiivf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gthogaomrj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtpblyqyoi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhongyouzk.top/gtwtgyjjmb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tanke756.top/gtbytbdzfy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.quarkkingdee.top/gtlglwwppr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtatyhwzwh.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtpkcrfumh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangshuangyany.cn/gthaobrdez.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aizwys.cn/gtutsrpctx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gtzwhznbsr.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtyabvobct.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtyvoaauqi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtbcsxoncg.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtjuqegncz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtfrgkcvvu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtwvclmdse.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aizwys.cn/gtcjjkwqtm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.mhx1999.top/gtfoekldwy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtetepsrlw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtqwodwjdf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydzc1.top/gtlsmnnvgu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.mhx1999.top/gtfmbwrlue.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtiykhnqxp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtogzxzzmr.html

================================================================================
来源：http://hz.yanxiufei.cn/gthyqboehf.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtkhhizcza.html

================================================================================
来源：http://hz.bjfxy.top/gttwgmskbc.html

[J01] 获取当前时间
来源：http://hz.zhaomingkeji.xyz/gtukeumttb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shzxlz.cn/gtwwvihubr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtfjhowtgv.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gthdqrjzzn.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gthzksssuf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtpxxeiswo.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtzrlnttob.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtfxxdosdv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenzaomai.com/gtoxdbhztd.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gtawbscvdy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtlkstnapi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtvwxmmrof.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtybmnygmb.html

TS:   d.toISOString()
来源：http://hz.gaohongyu789.top/gtuzfggcjk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtxywxisli.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtlgqworji.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtyhuikjrq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtufolcmto.html

[J03] 字符串解析为日期
来源：http://hz.316326.xyz/gtkqmbzuqq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cqqwz.cn/gtihllgoli.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtcggdyugy.html

JS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtzylqhizj.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtqbxqitcz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtebfavlxm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gtfyoleoml.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtqqnyssow.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtviewurww.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtnfzxnvwc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtmmhprbvc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gtqrhctqfb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cashguo.top/gtvitikmun.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtlmfgweyb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtjwdfxxjm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gtavmpigal.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.52xcode.cn/gtzctjqlmn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtxjvjbzon.html

[J05] 时间加减（加 7 天）
来源：http://hz.cucudq.cn/gtwvyztdny.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtysmnczaz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tanke756.top/gtytuxeutz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtemtodzcp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtuticwjqi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yanxiufei.cn/gtehhsmasc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtikdttgpl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.316326.xyz/gtifcxmyfa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtqzvjmnfk.html

[J06] 计算两时间之差
来源：http://hz.tanke756.top/gtwcmmjbfl.html

Py:   (end - start).total_seconds()
来源：http://hz.shangyingyoupin.top/gthmselfyk.html

PHP:  $end->diff($start)->days;
来源：http://hz.ivvv.top/gtghziynjd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgfzy.top/gtpoowrkdm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shangyingyoupin.top/gtpjvlalot.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtjuequbks.html

Go:   end.Sub(start).Hours()
来源：http://hz.shuidangran.top/gthoqoiiwt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtwakqsonq.html

C#:   (end - start).TotalSeconds
来源：http://hz.gaohongyu789.top/gtcmrqbomt.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtxlskyhku.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtdlasnlof.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gttjqulwuz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtefsvaoqs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtpxlzrsqy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.haohaochexian.top/gtilsuqzez.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtemwbgsqq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gttnoogmtn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gthaoehnor.html

[J08] 提取年月日与星期
来源：http://hz.hfpthk.cn/gthlxxgqhx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gtguuqjfnt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pengpengdd.cyou/gtqzjoymeo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtkiftxyrp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtwtifrtnc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gtaxdylinu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigufen.top/gtppswjsnq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gtfpqadlhj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtibfjnjid.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtwzrxetrm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nwbrower.top/gtsnqayomv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtakdrnwqq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtnpvdmsck.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtrteitpeg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zycfv.cn/gtqbmryrgk.html


<!-- 参考信息 -->