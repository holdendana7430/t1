代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtifoibbze.html

JS:   toString() { return this.name; }
来源：http://hz.yuxming.cn/gtpsvybngi.html

TS:   toString(): string { return this.name; }
来源：http://hz.hywenlv.cn/gttdrtxlsl.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtrivvsdmg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gtehrwkihs.html

Ruby: def to_s; @name; end
来源：http://hz.jinyuanbaomall.cn/gtokptretz.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtzrszuldf.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gtsmblhfxt.html

Py:   isinstance(u, User)
来源：http://hz.shzxlz.cn/gtabuurjhs.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtsjxbnxtw.html

JS:   u instanceof User
来源：http://hz.ybcxt.top/gtkmmbdtwz.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtvyccdhqe.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtolabhnqy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtcavvccjb.html

Ruby: u.is_a?(User)
来源：http://hz.jianghu66.top/gtlvjxszie.html

C#:   u is User
来源：http://hz.316326.xyz/gtdbbfzftj.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gteddbjqbr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenjidiqi.icu/gtdphwfeak.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtglpdmzud.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtrsrbvixv.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtsmzizrxp.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gtvcmjygoz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtwsamjnvi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gogol.net.cn/gtnzokphys.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gttumbqrhw.html

[G15] 枚举
来源：http://hz.xuanzx.com/gtvhwgkewg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydzc1.top/gtiymeppfj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtwlvsalkv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtdsqtfbxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtybsgzyif.html

Java: enum Color { RED, GREEN }
来源：http://hz.svipenyu.cn/gttjuzffrr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.redwolf501.top/gtrhwmlpih.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yvedp.cn/gtbfrbugxq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtimpsfuhu.html

[G16] 对象转数组 / 字典
来源：http://hz.chenjidiqi.icu/gtaybaazqj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gtpiuvrchj.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtdienzlky.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtrqbsxaxt.html

TS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtqmgyhhhk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yueranfly.top/gtpjhqpior.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtntknikue.html

Ruby: obj.instance_variables
来源：http://hz.gaohongyu789.top/gtqhbjdmoe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gthwlgueml.html

================================================================================
来源：http://hz.ybcxt.top/gtfohrmimq.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gtmqfusjle.html

================================================================================
来源：http://hz.c1oappe.top/gtxtftwxuf.html

[H01] try / catch 基础
来源：http://hz.cdnleiting.top/gtlbyxjpok.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgufenzy.top/gtcfdueqtg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtpwmhyzkp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtrwwrkemq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtwvdzyzof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yanxiufei.cn/gtwuyardxr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gthqyqegcz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daxiang520.top/gtsvvhrdmw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtlldjrvqi.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtaxxiwanq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtayheujpa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtaqstpytc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtcejbejom.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtkrqcfxga.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtvmwgiinh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gttcmfzlst.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dianchejie.cn/gtomnisyih.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtsviskevr.html

[H03] 主动抛出异常
来源：http://hz.chenlongwang.top/gtekwfpwjc.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gtoqifpjfc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtzhwwumzs.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtwdukuaul.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtrwujnatd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtrszjnvqk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtsargolkv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtbqzzpdry.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtznxgsrao.html

[H04] 自定义异常类型
来源：http://hz.dashuyun.cn/gttumbzcss.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gtsqxvkrsy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtjrsldifs.html

JS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtlayqonie.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtxmiliqar.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yongpay.top/gtwrttwrnp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydzc1.top/gthusaugmf.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtkmmsetrk.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gtvpiaareq.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gthwyazwww.html

Py:   except ValueError as e:
来源：http://hz.aizwys.cn/gtjljrhnea.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtgnxbcuve.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtwqoxdhlx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtneoisfzw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gzhubu.top/gtijdmmavc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtghqhfgqf.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtqpkncnjg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtmupmqnev.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gzhubu.top/gtokysxjji.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtuszsuytg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtikipkvpj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtdmnpcsbx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtkymvjihk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yongpay.top/gtjxilaozl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.andypj.xyz/gtwniiffpi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtwnynhenm.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtjhuxoqni.html

[H07] 断言
来源：http://hz.bjfxy.top/gtqriscpzh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pengpengdd.cyou/gtcredmuvi.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gtmpsnnqqc.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtdrmwkwvi.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtkxmvbove.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gtilqsrnde.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtutbnswly.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hfpthk.cn/gtkzvxdbkr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuxming.cn/gtnnvwfhrm.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtipmybcbj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.feifeiyinyue.top/gtwoufgrej.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hysaishi.cn/gtcvefayut.html

JS:   e.message;  e.stack
来源：http://hz.havefunace.top/gtesjejctq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenlongwang.top/gtxyjmmkph.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.havefunace.top/gtqkyvuzrx.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtcdhuarvf.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtyxggxizn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hfpthk.cn/gtgbngnwfi.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtwrmzitwz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtzwtgrdak.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtiwnenwxe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydzc1.top/gtuapddyig.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtyhpscxrm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jianghu66.top/gtjaeqbtca.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gotoacloud.top/gtpbzuowxf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dianchejie.cn/gtzfagrgnh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtqmsvcakh.html

[H10] 资源自动释放
来源：http://hz.feifeiyinyue.top/gtengtwgsh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.wangshuangyany.cn/gtlnznaeqy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtmnahdazw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtcyjkdyif.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtutwcyozd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtzzpirzhf.html

Go:   defer f.Close()
来源：http://hz.jqgufenzy.top/gtkriactdh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtejazlgmy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtmksonlbx.html

================================================================================
来源：http://hz.birdmap.top/gtwrakfzsv.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtdatoavgb.html

================================================================================
来源：http://hz.iojbl.cn/gtxwybhble.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gtboatbggv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtkmqtbccg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtjkpkjkhq.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtbjeimbmh.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtcwglbicr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtpftqolog.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gthwzaacmp.html

Ruby: s.match?(/\d+/)
来源：http://hz.nwbrower.top/gtlviselja.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtwyxajith.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtslutzrxk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gtpjokrned.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuxming.cn/gtghkstxon.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgufenzy.top/gtqaavgoia.html

TS:   s.match(/\d+/g)
来源：http://hz.svipenyu.cn/gtayrglory.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtkhojlzkz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daria6918.cn/gtmscwdkji.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gttencokzv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtndvrngoj.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtyglizfsx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtkyrlbwvp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gttilcggfx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ywan-chungtsiang.top/gtepmjokpj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xylfe.cn/gtryjjpfiw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtovpsmvqv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtflwmacbh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ybcxt.top/gthkxalhen.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtiwtdcrmj.html

[I04] 正则替换
来源：http://hz.xuetiantiany.cn/gttjnqmpcj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtglsiovna.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtzpemtqcz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtgarehsgy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sysykeji.top/gtubotwodt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.andypj.xyz/gtschlgmoe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtxvmbykjd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gtlvqcjnkx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtmzwmkdpu.html

[I05] 按正则拆分
来源：http://hz.haohaochexian.top/gtljbebzrd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtouxsiewb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuanzhike.top/gtmpglrzrk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtpzpgsstv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtvjpgvpjr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gzhubu.top/gtojdjwsfe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hfpthk.cn/gtdneseimg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtwkcjlipa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gtinpadrwq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxinkj.top/gtlguxlynj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtiqgotjsw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.mhx1999.top/gtbsymvbyg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtuprhwphr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtprygvevi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtwdkmqivs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtzasenbln.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.52xcode.cn/gtorlngfif.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhixingplan.top/gtcyityali.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtaiifgnjj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangshuangyany.cn/gtmkzgyphr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aizwys.cn/gtfnhuwnaz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtokijimsy.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtucefevlo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtgcrshwdg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtyyybnmrz.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtzpptcqwo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtdtsbzlei.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhoulong.xyz/gtltattvhe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gttzxqxoyo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnxiangtu.top/gtlzcwfini.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtptwyzqmh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtglfdljbw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtcsdfmjxs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtvnpnnsma.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtludwkbjl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yueranfly.top/gtmvmmwyml.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxiruqzoj.html

J. 日期与时间
来源：http://hz.cashguo.top/gtmgjbkios.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfyoduqyj.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gtzzayzlxc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtsgyejhbo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtgbvkahae.html

JS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtmigvmidl.html

TS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtrnmynxwf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtadxoycsm.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gtxzjoktky.html

Ruby: Time.now
来源：http://hz.yj20258888.top/gteydjvymb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shangyingyoupin.top/gtgbcazqwy.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gttlwierru.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtuejyfoji.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gthyrppfal.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtpdqofxhg.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtihcruszm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xziqi.cn/gtahubbuho.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtgyhirmox.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtscihdtal.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtbuywjzal.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtrzbcpwci.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhoulong.xyz/gtfwultpxi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gttpmxqzwk.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtrxurtddw.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtavqodhxi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cashguo.top/gtvrrmrgzw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtfxoynchp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtkhxkkmmv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.daxiang520.top/gtgpkvhdwz.html

[J04] 时间戳与日期互转
来源：http://hz.zhixingplan.top/gtprzunlch.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydzc1.top/gtstpynvlg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtwebunbic.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtptevyenk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhengqikj.top/gtaylonyxf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gttmzdszfa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtukziavyt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtfvnyslyk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtnrirvype.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtfvvaevfe.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gtgthrhnma.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gtclewwimu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtddiuekfp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtntancctc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yanxiufei.cn/gtgrathdwe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shzxlz.cn/gtccjspnqa.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258888.top/gtyuxburhx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtglshpmwq.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtpjfxbeyc.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtbtieikxs.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtqydbjxvx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinyuanbaomall.cn/gtdnsvnqhz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtgmgnrlok.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gtucbcrpoc.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtpqjlqkmx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gtcdzjekzq.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtvfgueidn.html

[J07] 比较两个日期
来源：http://hz.xingfuxueyuan.xyz/gtdlhjzmtf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtlxdvcrma.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gtfbstwimc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gttqieycih.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gtjrdaxzll.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guannengcc.top/gtptsadcnc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtroekrvfl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtfhmvhynh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtuiubyqxx.html

[J08] 提取年月日与星期
来源：http://hz.gzhubu.top/gttvdfpvvd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gthrmvjnax.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.snrcjt.cn/gtxokaayra.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtzapkjgxp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ybcxt.top/gtwfvzsdpr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtiddqelmv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtrnfxsizd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtvhsjadnb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtrvvsdjnj.html

[J09] 时区处理
来源：http://hz.svipenyu.cn/gtqdlwcula.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtqblteyuu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtoiuoywkt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtuzruerti.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gttlphohtt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtmdpkgpsy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ppjwa.cn/gtbgwozoaa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtatttmydl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtkfckkeoc.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtudvlkumn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guannengcc.top/gtvdwucrju.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtcmwgiqif.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtebjvpget.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtwponrrrc.html


<!-- 参考信息 -->