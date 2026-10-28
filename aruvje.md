代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtwrtbcoty.html

[G11] getter / setter
来源：http://hz.hywenlv.cn/gtmdrbtagp.html

Py:   @property 与 @x.setter
来源：http://hz.cdnleiting.top/gttftoehpz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtnofgylwl.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtgislrfyj.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtmyiectey.html

Java: public String getName() { return name; }
来源：http://hz.xziqi.cn/gtamchlqbi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtfzcdjxel.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtelxqgrgg.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtuvkxyfpn.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtaktsfpze.html

Py:   def __str__(self): return self.name
来源：http://hz.zhijiandao.cn/gtcbqjenlt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtcgacsrqd.html

JS:   toString() { return this.name; }
来源：http://hz.52xcode.cn/gtfiprfcho.html

TS:   toString(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtiiyztowb.html

Java: @Override public String toString() { return name; }
来源：http://hz.jianghu66.top/gtiemphyqb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gogol.net.cn/gtqbxrecmo.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gtxazfdsmh.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gtocezlgqb.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtkglervkb.html

Py:   isinstance(u, User)
来源：http://hz.jinghuilouyu.cn/gtxfhbztor.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtqlhyyoze.html

JS:   u instanceof User
来源：http://hz.iojbl.cn/gtcybhbtgx.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtaqjcgaoy.html

Java: u instanceof User
来源：http://hz.cheryme.top/gtmtevljhp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtdvdwcdgt.html

Ruby: u.is_a?(User)
来源：http://hz.hnqzz.top/gtsyvykuke.html

C#:   u is User
来源：http://hz.ybcxt.top/gtdiochcuc.html

[G14] 数据类 / record
来源：http://hz.yueranfly.top/gtfolphvnq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtxweijwmg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guowangkeji.top/gthyzknoed.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtzirgcaca.html

TS:   type User = { name: string; age: number };
来源：http://hz.fengsongda.top/gtrbowytey.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtetwymrji.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258.top/gtumkhcqdi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuanzx.com/gtgieqndxf.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtqubdosmw.html

[G15] 枚举
来源：http://hz.iojbl.cn/gtpdqamgef.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtwykahdgz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtfayfhxlm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtalddmkwt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtlkulzibd.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtbpaimnin.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gtgymvdcjj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtlnmzbfuo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtdvlwqgmq.html

[G16] 对象转数组 / 字典
来源：http://hz.yonumen.top/gtazbfvnuz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gtdvrjzfxk.html

PHP:  get_object_vars($obj);
来源：http://hz.ydjk.org.cn/gtadjcvewj.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtfpcthbor.html

TS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtsxlerfsz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtbbxxsnxe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtzjrixlmb.html

Ruby: obj.instance_variables
来源：http://hz.xuanzx.com/gtgvpzsqqa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtotumslaa.html

================================================================================
来源：http://hz.pycfn.com/gtxxplsijp.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtbmzfnwir.html

================================================================================
来源：http://hz.hysaishi.cn/gtyjhtbibi.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtbouxpscz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtgdoiyupj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nwbrower.top/gtvanyrxwb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtxrlcqkuu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jiagoushi.top/gtzyuwhbve.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtxtriloou.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtlrauyzpd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.c1oappe.top/gtkgeycota.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtxufgnbwx.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtcqkntvmz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtciyzmtfu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtdaqezbab.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtbulzbrlr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtjhckbjyt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gthargjepl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtjbbnfscq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zdqjudy.top/gtxcnmnzln.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtpatbidlq.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtkinwgsnk.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtrgqurnuf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtpcqkqtnb.html

JS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtoojkjybl.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gttjyvfejl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtqcnhgqhv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtekqpwndm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtlynosvde.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtyotmapvx.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtzzbzyoej.html

Py:   class MyError(Exception): pass
来源：http://hz.meibo888.top/gtiqmgtswi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtotqlyono.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtwpfiuhgs.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtzzkvjzml.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtnxakbodl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gtokxytllg.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtfxsgzznj.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtapikhgjb.html

[H05] 捕获特定类型
来源：http://hz.yj20258888.top/gtsohzqwfz.html

Py:   except ValueError as e:
来源：http://hz.9152youxi.cn/gtleocpsas.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtyubgyjal.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtbxnwkrdh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtdqlplppf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guowangkeji.top/gtwzueuojn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gtjhapdmuc.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuanzx.com/gtdvtepzea.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gtfawfhalc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jlsjyb.cn/gtxkevwsch.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtjdbiwaqc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtoqfmyklb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtcxbspcup.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtrouittsa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gteerjjxkp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jiagoushi.top/gtzebzwpjn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gthkameayh.html

C#:   obj?.A?.B ?? default
来源：http://hz.yueranfly.top/gttaftojoe.html

[H07] 断言
来源：http://hz.zhongyouzk.top/gtqmdlzwui.html

Py:   assert x > 0, "必须为正"
来源：http://hz.kuanghao11.cn/gtzqotafhz.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtsibsmcsf.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtkgplwglb.html

TS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtkrbcrchp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gtyvoqjrzr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtwzlyvuuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aizwys.cn/gtnlflxzkl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtkpnijrnp.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtyiwelggj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtnsmgxnwz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtwwfyhxjn.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gtlowyxkuo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtssqwwijn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258.top/gtvsemsmyd.html

Go:   err.Error()
来源：http://hz.zhoulong.xyz/gthmgnovvm.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtcjeqiczp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtobgodldz.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtubyenosm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hongshengwenyu.top/gtywtopgdi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gttjlbhcdx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtulinvhsu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtnxvwgjjf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtmjieneyb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tianlin.xyz/gtdazzmqpn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtcqybqrrf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtgxnmdxwl.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gtrayqsqnp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtsvudivuj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nwbrower.top/gtwsqykply.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtcmmltooo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtdatvbldi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuanzhike.top/gtwycsdvkv.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtbaehigpd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.meibo888.top/gtnjgkxcia.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shzxlz.cn/gtmevtfcja.html

================================================================================
来源：http://hz.yvedp.cn/gtjafogiui.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtsuljxgjs.html

================================================================================
来源：http://hz.yangfankeji.com/gtumbmgyka.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtijqupqpn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtqskihsei.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sweek.top/gthgubfjyj.html

JS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtyrujplei.html

TS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtwcewnuwl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ywan-chungtsiang.top/gtdchsiddd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydzc1.top/gtmpgypcww.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtqxkdsnhi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zdqjudy.top/gtnckhfqbj.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gtrjtsbiye.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxuanxn.top/gtibfdtpdr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gtvzlcdfuj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtilgdjppy.html

TS:   s.match(/\d+/g)
来源：http://hz.ehwqpu.com/gtsunxjwbw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnxiangtu.top/gtbgvywdjj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gaohongyu789.top/gtmhmbtnis.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtfzdmhnrn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pycfn.com/gtuzjiaels.html

[I03] 提取捕获分组
来源：http://hz.yuxming.cn/gtromcxnsv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gzhubu.top/gttkhfkuru.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtjaymdnrr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtplrvbbqu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydjk.org.cn/gthrqxxfrq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtuhxyotgz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yanxiufei.cn/gtuwkpvqjq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtokclwjxm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gteaecpfgj.html

[I04] 正则替换
来源：http://hz.cashguo.top/gtybghefvr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gaohongyu789.top/gtjknckbmk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtnjbmndxs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtdmqxzkdr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtjojmeuot.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtubqnbnvd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtvvclebrh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtrkkyqucs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gttbhmphcz.html

[I05] 按正则拆分
来源：http://hz.fengsongda.top/gtizbdtbqu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gotoacloud.top/gtjsvtxpyu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dashuyun.cn/gtvzbhmbyq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtbpfwxotm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtvdvcxmfj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jyoumei.cn/gtqqmmthmv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtjruvxgvr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gttqssnvgv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sweek.top/gtlinqazuy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtlxgdeffp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtnvapirrb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtrozcendb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtrnidtmwo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtixdpoocc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gtjnwdrpzn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuanzhike.top/gtndqehbac.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gtwkxryvsl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtsjuuwkni.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gtejzheipp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.svipenyu.cn/gtkcmuwaut.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hongshengwenyu.top/gttyayvjbf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dianchejie.cn/gthqoyvsnb.html

TS:   /error/gim
来源：http://hz.9152youxi.cn/gtmwjcqdzu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yanxiufei.cn/gtvxqrabwu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangkeji.top/gtvwaumtzm.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtfpybjnxt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhongyouzk.top/gtwrmufmwc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtdryfayzr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.redwolf501.top/gtnjujmbqd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtvnzmlnyv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtpokkeomi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtiujtcjlu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtqahyaied.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtzfuggfay.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gtbkcbowlv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtscmsrewk.html

================================================================================
来源：http://hz.xinyue.icu/gtvlxjqmbl.html

J. 日期与时间
来源：http://hz.sufxvd.cn/gtjwywvjkf.html

================================================================================
来源：http://hz.cdnleiting.top/gtendhlamz.html

[J01] 获取当前时间
来源：http://hz.jinqigfzy.top/gtnuhpjdby.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtoqblmiwf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gthcprjure.html

JS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtfgebucoy.html

TS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gthubbcejf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gtskgxihuf.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gtzoyiizqz.html

Ruby: Time.now
来源：http://hz.hnqzz.top/gtgnoqipki.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shuidangran.top/gttwjlmnsw.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtnllzswdz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtseyxqcep.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtqcuqtqvl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.0kj1m.cn/gtgklmnzbj.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtczglcdxv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jianghu66.top/gtqoardrqk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtamqruesv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gtcxixpahp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtshfmtwrx.html

[J03] 字符串解析为日期
来源：http://hz.vqdsnc.cn/gtiwsktnri.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tian-w.cn/gtmgofiayr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gtrrljhqvl.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtvdplmclv.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtxdiwsbck.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtqvkgaibh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtfvuomncv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtnwgjkfwi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258.top/gtpwwkmiuo.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gtfpflfmzc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hfpthk.cn/gtxbzyszcu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gtgbezhlpy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gthbexsabz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tian-w.cn/gtvzmyctrb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hfpthk.cn/gtbhumaerv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cheryme.top/gtxezhkuce.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yueranfly.top/gtgmynmndz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtqizbosrv.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gtpdmfddur.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtqasaorkz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtujpfluyg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gthpmuhcgb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtkqusghds.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnqzz.top/gthyibuovg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxuanxn.top/gtuelbfjuc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtqqwsxyrh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtsphfnrya.html

[J06] 计算两时间之差
来源：http://hz.yonumen.top/gtbonxxkqj.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtwjdeijrr.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtfxmqtfkl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gtaeuiraul.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtclgwngpc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gotoacloud.top/gtkcbvobqg.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtxljrhica.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtgewcjavt.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gtvflskcks.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gtjksibdff.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtcsotjsfd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigufen.top/gtdjgnrmac.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtyoxfdmao.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtrfrfzgzj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sufxvd.cn/gtwnwujvbm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhiwuduotai.top/gtrjjjpmwq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtaiceolpa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtqumojdqf.html

[J08] 提取年月日与星期
来源：http://hz.sysykeji.top/gtjstexxti.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtzcjpgwfs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fzhhl.top/gtpflqrilt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gogol.net.cn/gtrmsxnwcy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangshuangyany.cn/gtjaadkrql.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xinyue.icu/gtxrcaivcw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtugmugcav.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.redwolf501.top/gtbltsudst.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtfzdnxrtn.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtvumkuetg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuetiantiany.cn/gtghbiqnoa.html


<!-- 参考信息 -->