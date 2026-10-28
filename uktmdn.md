代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.jqgufenzy.top/gtpgkpwajq.html

TS:   get name(): string { return this._name; }
来源：http://hz.9152youxi.cn/gttyrgkvon.html

Java: public String getName() { return name; }
来源：http://hz.shzxlz.cn/gtvtgnbfld.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.snrcjt.cn/gthdhrkquq.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gthuebyyfa.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtqsugfjvf.html

[G12] 对象转字符串
来源：http://hz.birdmap.top/gtnrzzsape.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtmpkpkmio.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aizwys.cn/gttnsizmkq.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtobtpcgfm.html

TS:   toString(): string { return this.name; }
来源：http://hz.yongpay.top/gtfllvryvy.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtjptipwde.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtfwxxrdjv.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtzpfozjsm.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtbyvbdymy.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtekuoqcwe.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gthdbpczko.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtxfutqtey.html

JS:   u instanceof User
来源：http://hz.sweek.top/gtnowkfzta.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtrpciscyt.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtfogvxdmv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnxiangtu.top/gtnecdztgl.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gttqpaggrv.html

C#:   u is User
来源：http://hz.birdmap.top/gtuncrcvkx.html

[G14] 数据类 / record
来源：http://hz.guowangkeji.top/gtlhhtucdt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtibnxqkcz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gttjzmrpov.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hfpthk.cn/gtfsfgzhyf.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gtftiipxuw.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtvocbdqfl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shangyingyoupin.top/gtekjadyni.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtplzeheop.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gtvxrxcxzi.html

[G15] 枚举
来源：http://hz.smart0.xyz/gttuwndbkj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtcnjlozac.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hongshengwenyu.top/gtwvhourse.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtizfkadta.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtjcdidtog.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtmqjgmffc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtkbmnuyka.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtzagerhcq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtcpopvocb.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtxicpwuzb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gteuhqlzrb.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtcpylcswj.html

JS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gttbyzafjp.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtvxvzmcep.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fengsongda.top/gtjrhafenk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.vqdsnc.cn/gtlimmjbby.html

Ruby: obj.instance_variables
来源：http://hz.tanke756.top/gtgxangxdc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.haohaochexian.top/gtcehhgajo.html

================================================================================
来源：http://hz.hnqzz.top/gtuhqodzji.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtepdslorr.html

================================================================================
来源：http://hz.birdmap.top/gtyjtmtrih.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtbolibwwu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtrmlhipqe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxinkj.top/gtjgptaswq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtpyrwowle.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cashguo.top/gtyypxwzzl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.meibo888.top/gtffueiesh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tianlin.xyz/gtpeyvixpp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.feifeiyinyue.top/gtlvtqznqt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.andypj.xyz/gtjksrarde.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtjosercpb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xziqi.cn/gtdtsfhpeb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtsryrkdpa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtogsobkgq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtrpcxalbt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtehypmmmw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xylfe.cn/gtnmrqedxv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtqlcrbelu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gtevxgcyno.html

[H03] 主动抛出异常
来源：http://hz.ppjwa.cn/gtpizmbgie.html

Py:   raise ValueError("错误信息")
来源：http://hz.gzhubu.top/gtuoltdcho.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtghxaqplv.html

JS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtsfjafpii.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtlznovvcf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtwokayezu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtqhnlgdkw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigufen.top/gteamybkpl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj202588.top/gtqbghbdwd.html

[H04] 自定义异常类型
来源：http://hz.hywenlv.cn/gtlqmqnunu.html

Py:   class MyError(Exception): pass
来源：http://hz.jianghu66.top/gtkmksuvko.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtmtvlnlgj.html

JS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtmcnchnvw.html

TS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtwwshzhlt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtkbsppndh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinghuilouyu.cn/gtrycbqltz.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gtvhgggsju.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtfukedthw.html

[H05] 捕获特定类型
来源：http://hz.yj202588.top/gtqcbhkpih.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtsltyblvi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtimezigwu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtyylroaer.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtzqmrbgck.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gthkexiiqg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgufenzy.top/gtpfmysooy.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtloqgkdwt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gotoacloud.top/gtdyrzlncc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gotoacloud.top/gtdjypkqrs.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gttybtjhtz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.mhx1999.top/gtkxjeliwm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtwjimqnyv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtjvcajgnf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gtarubnhjw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtsjaukgnr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xingfuxueyuan.xyz/gtqlpiugjx.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtdrlvusjb.html

[H07] 断言
来源：http://hz.zdqjudy.top/gtozvlozzh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxuanxn.top/gtmomnlktg.html

PHP:  assert($x > 0);
来源：http://hz.yuanzhike.top/gtsldvslcz.html

JS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gttphhozew.html

TS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtocimjthh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gttcbjujot.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hywenlv.cn/gttcfbzfru.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtydzgqeeu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gtdnvtufwc.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtxipxvosd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtncezrubz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.redwolf501.top/gtdczgvkku.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gtgvrhrwxl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtrembvnci.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtrnsxlqdf.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gtjwhicrqy.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtegsegpgf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtmapfrgnd.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtydfskkqr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtmdhknhhb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtmeronwel.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gogol.net.cn/gtpfiyvkrf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.316326.xyz/gtquvjjzgm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cashguo.top/gtxrgxensv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tian-w.cn/gtytzqensl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gteheoczdh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jiagoushi.top/gtuidkxiau.html

[H10] 资源自动释放
来源：http://hz.xuanzx.com/gtlkyoyzns.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.316326.xyz/gtntxogowu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenzaomai.com/gtfnaptnke.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtitsdtzsw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtrkjlywmr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xingfuxueyuan.xyz/gtceuyztks.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gtktovdkcy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shzxlz.cn/gtmbzbbzvy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gttckznkpf.html

================================================================================
来源：http://hz.meibo888.top/gtugcohmxv.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtbnokdhgt.html

================================================================================
来源：http://hz.ydzc1.top/gtcgurzdzo.html

[I01] 判断是否匹配
来源：http://hz.shzxlz.cn/gtjbozdxgd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gthxnhdzdk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gteryyvzhy.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtpakjfiqu.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtsipcbkrh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtjosydxqn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hfpthk.cn/gtwbpxoktv.html

Ruby: s.match?(/\d+/)
来源：http://hz.xziqi.cn/gtjogfnbkx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gthlekujws.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtfblffrsa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtqtfipmpq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtnsynqcot.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.snrcjt.cn/gtoztwcxwl.html

TS:   s.match(/\d+/g)
来源：http://hz.feifeiyinyue.top/gthzekabob.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtfmlkustb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.kuanghao11.cn/gtroippnst.html

Ruby: s.scan(/\d+/)
来源：http://hz.quarkkingdee.top/gtqjdfwvmc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aizwys.cn/gtarwineur.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gtzjtmcmrv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangdashe.top/gtfudxdbrl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtqwwttjdo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtubitbjur.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shangyingyoupin.top/gtabtyabsm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtupwqavpq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenlongwang.top/gtsafxybbl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtbkqmbdni.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gtnwxwrgfm.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtixrhlzwd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.birdmap.top/gtejrupvph.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtznakjauo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtogmfybuk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtcrwkcqaw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydzc1.top/gtzxfklvjn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtkplgwpmh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtwmnwysvq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtwbaratja.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gttpbgegoe.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtgnkgeqdd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtvgqjqzle.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtwjtuwrqo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtakahgtqq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xylfe.cn/gtizvzzcll.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gtyoqlyowe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtwiawsyro.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gotoacloud.top/gtsxufcrtm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gteifjjwkg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtvbfcyfzs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangshuangyany.cn/gtzkgxctip.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtcectumck.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtnfxpprem.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtqxixytnw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gtdtozkspq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aizwys.cn/gtsmigxolm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtkzaforxs.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtcgsgefnr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daria6918.cn/gtjypvxdbw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gtujzfdbfi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hysaishi.cn/gtybowbqzu.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtfnsaqzap.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtealjsssy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuxming.cn/gttcfbvysm.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtkbxblmdd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.redwolf501.top/gtycpfqbha.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shuidangran.top/gtceugzzvg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtsxypxvyr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtudzjuxnm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtrxozxebl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtxjeszszt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtizfhdfai.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj202588.top/gtwkopsipo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gthrlznyzc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtocmeartr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpyrvpgxw.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtbifsfucb.html

================================================================================
来源：http://hz.hnxiangtu.top/gtkskpedeo.html

[J01] 获取当前时间
来源：http://hz.zycfv.cn/gtpqypbzmz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pengpengdd.cyou/gtcpthnrnh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtyddoepxc.html

JS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtsawabwqg.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtyyuedlnz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtzvvluovw.html

Go:   time.Now()
来源：http://hz.zdqjudy.top/gtfhztqfjk.html

Ruby: Time.now
来源：http://hz.yj202588.top/gtvagfhihn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ppjwa.cn/gtqwjuwtjz.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtmfbulcgx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtkzydbypg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtidtclggb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yonumen.top/gtdumimigx.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtjiqiwcvi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtdgrjcddt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtwqculzhz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtymtwjltq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gtqckhbvbd.html

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtnfdzvlva.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tianlin.xyz/gtxgpqoobd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258.top/gtjhcnutss.html

JS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtzthirlij.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtpdzixefn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtfxburwgr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtwpkilppb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtiqvizygh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtnbulxbue.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtsunrjjuf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtuwyaoljq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.meibo888.top/gtvpbnvzmz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtuyndfuiz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtlrcfyfho.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gtxgenepez.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gogol.net.cn/gtfhdwerxf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gtvuusdyjx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxinkj.top/gtchzitaka.html

[J05] 时间加减（加 7 天）
来源：http://hz.dashuyun.cn/gtxtxtbzop.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtszvhhkis.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtpntjvfuh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gteuwtqqqx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtarozzddd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.redwolf501.top/gtmzbgsxdu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.redwolf501.top/gtzhjbzovl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gtkujxfczz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtrdktajio.html

[J06] 计算两时间之差
来源：http://hz.guannengcc.top/gtvbeqvltc.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtmoeqlolm.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtyhnbtote.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtxlqhxvnw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtujpatdgv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hfpthk.cn/gtafidfoko.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtjyckcqnc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cdnleiting.top/gtwwgcyzoc.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gteceldtop.html

[J07] 比较两个日期
来源：http://hz.ivvv.top/gtdkhdpxfz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtvkhqwczp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gthbmzjtjc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtlnjgkpce.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtlcncfbnp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhiwuduotai.top/gtzzdaagar.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtwhjxtpaq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtqiekgtle.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtvktsjpec.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtydkwsyzv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtstyjiyph.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shangyingyoupin.top/gtzqeafdpw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hammf.cn/gthezhzzyn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtqcbghpyu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtlzfxvdel.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtcwdmyyiy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhijiandao.cn/gtiindybls.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yuanzhike.top/gtupkbbghp.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtdnaleggf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtojhzqksc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtmjjblkmv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtlxgrzpkt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtktoorsiz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtzzjcvuqy.html


<!-- 参考信息 -->