代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.0kj1m.cn/gtoenhmgut.html

C#:   public string Name { get; set; }
来源：http://hz.birdmap.top/gtutgouisv.html

[G12] 对象转字符串
来源：http://hz.9152youxi.cn/gtcpizcujy.html

Py:   def __str__(self): return self.name
来源：http://hz.ppjwa.cn/gtpoawxyjp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtmuoikack.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtphrnmjip.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtkzhinqvg.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gtuxwdqrsq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtvewqrabg.html

Ruby: def to_s; @name; end
来源：http://hz.zycfv.cn/gtfiirypfw.html

C#:   public override string ToString() => Name;
来源：http://hz.zdqjudy.top/gtifvvxeai.html

[G13] 判断对象类型
来源：http://hz.gotoacloud.top/gtqdkyuaqa.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gtyhnsgmnb.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtcglqryuf.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtmyzjopxg.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gttyzojegl.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtbdxlpgeb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cashguo.top/gtfityxfkt.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtcprrtiid.html

C#:   u is User
来源：http://hz.gogol.net.cn/gtofjjkuia.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gthyivbuzm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtkltfpupr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guannengcc.top/gtqyseojfe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtmicxyfoc.html

TS:   type User = { name: string; age: number };
来源：http://hz.pengpengdd.cyou/gthvpuxanl.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtryqgxhys.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtidqbwkru.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuxming.cn/gtejqskzhv.html

C#:   record User(string Name, int Age);
来源：http://hz.zycfv.cn/gtpkncsqms.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gthbrzrakx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.quarkkingdee.top/gtetvhhdin.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gtiavtaqqw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtulhwsovf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gtahrbvgih.html

Java: enum Color { RED, GREEN }
来源：http://hz.guowangkeji.top/gtmrywipsh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gteygeddtp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.birdmap.top/gtowlhmwhs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtkxjvfrma.html

[G16] 对象转数组 / 字典
来源：http://hz.snrcjt.cn/gtcqfewkpq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gogol.net.cn/gtysulpkgr.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gttttczwei.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtexnweyob.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtgtnqfytn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtlqmjnfip.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jyoumei.cn/gthuwufxyg.html

Ruby: obj.instance_variables
来源：http://hz.pycfn.com/gtdzqukppe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtbxleviqx.html

================================================================================
来源：http://hz.ppjwa.cn/gtqnbxyerz.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gthnyfymto.html

================================================================================
来源：http://hz.sxryk.cn/gthdlxnfje.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtqfjveedt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ivvv.top/gtzhujqaou.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinghuilouyu.cn/gtpyrjzziw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtzezfxxrv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtgiivsmuz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtkuupapyo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinqigufen.top/gtjgqhmglf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtnnysejdi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cqqwz.cn/gttqduxznb.html

[H02] finally / ensure 收尾
来源：http://hz.iojbl.cn/gtmdegfees.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.havefunace.top/gtejoiywdj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtftfedoev.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtjxqmlcht.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtexhxafdg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtdgzxscki.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.vqdsnc.cn/gtqrimffdo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dashuyun.cn/gtdtkkvnoq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtaukbpuip.html

[H03] 主动抛出异常
来源：http://hz.jiagoushi.top/gtbdadatkj.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtcxujokiy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gthrognvos.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtmkoyhcxf.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gthypzebmf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtwdayxpln.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gtapajtwol.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtsafdmmoq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtnddbdizy.html

[H04] 自定义异常类型
来源：http://hz.ivvv.top/gtvhcsnaop.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gttbwaixct.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtazqwhpdb.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtxlaxunqt.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gthpkjzfkz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tanke756.top/gtzqzwygbl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cashguo.top/gtloadqorb.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtgiuiyufw.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtuauvcdwb.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtqaamxlar.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gtvoiejnhf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtsehwufxe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtoburyath.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtndypfloc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gtdbsiackh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nwbrower.top/gtmrtogcap.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtwrtzgqkl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gttadouebl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtxdrxkiem.html

Py:   value = d.get("k") or default
来源：http://hz.hammf.cn/gtpzlggdga.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guannengcc.top/gtnjgwxoid.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtjrbfhgif.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtappfttag.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yvedp.cn/gtdhkxmmpi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gtzejmpqdf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtgyqnnwvs.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtmngqbxkd.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtyklultye.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gteaptsjzf.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gtovvhszfk.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtoxrcxzip.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gteeonuvbk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhaomingkeji.xyz/gtxkgjeevn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shzxlz.cn/gtdnyjdiyj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cqqwz.cn/gtincapkgu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtlomhqtqi.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangdashe.top/gtzjxfloak.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guannengcc.top/gtwxrypyre.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtvniilymw.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtkorbbusr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtrogbavft.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtsrabsbzh.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtadlkuphd.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtmzhdvppe.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtskgdhois.html

[H09] 带错误码的异常
来源：http://hz.sysykeji.top/gtlzscuiop.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtpbnznhwu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gtizlsevyz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtehghjlka.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtcrikjjci.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gotoacloud.top/gtxfnnjinv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtsljeivxx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gtwzzrvspl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gtgkacvmau.html

[H10] 资源自动释放
来源：http://hz.ywan-chungtsiang.top/gtzdqeupgb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtgoasluxj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtejursyyd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtmbwmydla.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtvenwnucv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jianghu66.top/gteaphpwvm.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtdgjmsbfm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtlinuvqck.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shzxlz.cn/gtkdgznzhz.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtlccgmyho.html

I. 正则表达式
来源：http://hz.yj20258.top/gtdztevzbi.html

================================================================================
来源：http://hz.cqqwz.cn/gtjzztwdsz.html

[I01] 判断是否匹配
来源：http://hz.daxiang520.top/gtrtdyiznb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fengsongda.top/gtrhcpjjpc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ybcxt.top/gtswfoblgm.html

JS:   /\d+/.test(s)
来源：http://hz.bjfxy.top/gtdzzokrfy.html

TS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtrbpekaxc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fengsongda.top/gtktjzeuxf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dashuyun.cn/gtgrptifud.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gthlojpdil.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yongpay.top/gtjptpzkiq.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtmtkdpbph.html

Py:   re.findall(r"\d+", s)
来源：http://hz.smart0.xyz/gtkbstuazi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cdnleiting.top/gtoysfwdct.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gttpowuxuf.html

TS:   s.match(/\d+/g)
来源：http://hz.c1oappe.top/gtuqomafdj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtxeaezdoh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.andypj.xyz/gthmeolbez.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtrpffamle.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.havefunace.top/gtozlmumps.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gthylhtjin.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtuideepuy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gthfsjgrfg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtkifqywzw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtzywkglpb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtrwgbddhz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtzvlzhsfy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gotoacloud.top/gtstaogddy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.vqdsnc.cn/gtpmmdykgc.html

[I04] 正则替换
来源：http://hz.316326.xyz/gtzweecuuh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gtddliybhy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gthmkkftdg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtfhtchpgf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gttpgvkcnj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gteghfwepp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.redwolf501.top/gtxhlizrnq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtjsdvuyxm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gtwqvxudsm.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtfydfncmq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgufenzy.top/gtapabhnqg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtmqyblmxg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtlxxemdyx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtvuwtlcmi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtoxtsrqsc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtwuldrzzz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtwojjbjis.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtyhksxoci.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.c1oappe.top/gtlyyxxtpo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtrreeiqfo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtzylbsoow.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtaphhmtsl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtczaramhr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shzxlz.cn/gtpndsdjdy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gtslpbmhey.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dianchejie.cn/gtotkomjch.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtuzglywku.html

[I07] 忽略大小写与多行模式
来源：http://hz.jyoumei.cn/gtqzprwpoi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtfiamybdl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zdqjudy.top/gtppjwtbgy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtupnbxbmk.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtrwndebez.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtkrswjgod.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tianlin.xyz/gtrpffmibc.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtgzkgfhzp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fengsongda.top/gtidhvxugv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dashuyun.cn/gtipmmtqxt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hfpthk.cn/gtmwstgfcu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xziqi.cn/gtowicibmc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtocmcypuv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtrlgooyyu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gtiiuijkbz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtsyrpuusc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daxiang520.top/gtfvvmpxae.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.redwolf501.top/gtzjktpmox.html

================================================================================
来源：http://hz.chenlongwang.top/gtfiuqapss.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gteiwvsjin.html

================================================================================
来源：http://hz.cqqwz.cn/gtforfszfa.html

[J01] 获取当前时间
来源：http://hz.ivvv.top/gtezeozwrl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hfpthk.cn/gtxerqcsok.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtmastwdus.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtfkhigxqj.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtsatqddpr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtzvzyikkm.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtuhfndkwg.html

Ruby: Time.now
来源：http://hz.jqgfzy.top/gtoflzblxb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtczhtxjgf.html

[J02] 格式化输出
来源：http://hz.cashguo.top/gtrknflbbo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtymfrxvzm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtazsvifrx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtukkxjxmu.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gthegfjflx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gtuwtqqntg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtfxyhfybr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtnkhpggmc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gtrukamjhj.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gttldsvfge.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtjznwslbj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtdfajuyqy.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtqnqbmjrg.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtnmfegvnb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtrbihctvr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtjgnaocvt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtgtyzutwu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtkrirqqhu.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtnvdwxynl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangtech.top/gtpnunvwmk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtacweumae.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.0kj1m.cn/gthxaogmsp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtttilyphb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj202588.top/gtseghnoxl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtpdassacj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtpjnvsrpy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtqyoqfcau.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gtorcaefoq.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtddakddpd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtdrlohliw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtycbfqgjk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtugtsikvf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtdxzdawcx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangtech.top/gtoleyrabq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yangfankeji.com/gtwhssfqvs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenzaomai.com/gtlstehuxb.html

[J06] 计算两时间之差
来源：http://hz.ydjk.org.cn/gtbdfbaxun.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtwzrsbrpg.html

PHP:  $end->diff($start)->days;
来源：http://hz.guannengcc.top/gtmylfybcb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhaomingkeji.xyz/gtbcnktdgw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtuvwtcxgj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gttmsutdfh.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtekkifaqq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtimgsqgnl.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtainecdiv.html

[J07] 比较两个日期
来源：http://hz.xingfuxueyuan.xyz/gtgmiijkmo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtdsaatxxx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gtgpkanxpc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtnmjjfcrw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gttlmzkskf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xingfuxueyuan.xyz/gtifcwdady.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.feifeiyinyue.top/gtoknqkayq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtzafmltta.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtwzwxemvx.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gttjshjrjo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtyfthserf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtzxssvzvk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtlslsbkcj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jiagoushi.top/gtkmxugbzv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtmctwzfwn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aizwys.cn/gtvjkdazbb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtcanosccc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yangfankeji.com/gtqjablkho.html

[J09] 时区处理
来源：http://hz.feifeiyinyue.top/gtlsxpxnvy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fzhhl.top/gtoijghayn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yvedp.cn/gtyrpkorym.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtwnbfgpfz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtcfdqxbtz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gtavfhxzlu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtanyiyqty.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtirvavdwu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gtrichqyts.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtmqrvxsyw.html


<!-- 参考信息 -->