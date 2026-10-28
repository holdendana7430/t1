代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtmpbwsqxf.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtndfshhcz.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtxpjipffo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtiwptsqbm.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtnmvbcfsh.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtramoptpp.html

[G12] 对象转字符串
来源：http://hz.shzxlz.cn/gtgxcwquyv.html

Py:   def __str__(self): return self.name
来源：http://hz.ydjk.org.cn/gtictrbprr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtwavqquru.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gtygdcjbit.html

TS:   toString(): string { return this.name; }
来源：http://hz.sweek.top/gttoghbpdu.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gtfjmltkym.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtpwkhzivy.html

Ruby: def to_s; @name; end
来源：http://hz.ppjwa.cn/gththxrnpc.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtbzhhusuv.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtdgxzpxks.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtrtbmyfbw.html

PHP:  $u instanceof User
来源：http://hz.iojbl.cn/gtxyloqwqy.html

JS:   u instanceof User
来源：http://hz.shzxlz.cn/gtenjmshmj.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtmazgijid.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gtmbpqzyld.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gtveafnqyz.html

Ruby: u.is_a?(User)
来源：http://hz.gotoacloud.top/gtsvpxsqog.html

C#:   u is User
来源：http://hz.guannengcc.top/gtbwnqqumv.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtifktxgds.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtzouohqvn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtdtgcbgjh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenjidiqi.icu/gtnckdcunb.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangdashe.top/gtmkjzpkwd.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtxgbdfjka.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gttoceijvl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.kuanghao11.cn/gttfimqtyv.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtyywgjldz.html

[G15] 枚举
来源：http://hz.sufxvd.cn/gtwqnvecgt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gtzytyuafn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pycfn.com/gtnftvshwk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtcfjqavct.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtnkljrlnj.html

Java: enum Color { RED, GREEN }
来源：http://hz.dianchejie.cn/gtvjbcaxnp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gotoacloud.top/gtxgabqpfc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtgsyiybfy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtxukhafhn.html

[G16] 对象转数组 / 字典
来源：http://hz.shuidangran.top/gtyekerqdw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtslbypdfg.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtcnwehjmh.html

JS:   Object.entries(obj)
来源：http://hz.pengpengdd.cyou/gtrekpxkcw.html

TS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtzkvvhiou.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cqqwz.cn/gtqaaypfcb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydjk.org.cn/gtlcldsmoc.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gttneoarhk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dianchejie.cn/gtnkinunfe.html

================================================================================
来源：http://hz.bjfxy.top/gtjhmemprj.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gthjwgjjll.html

================================================================================
来源：http://hz.ivvv.top/gtljiljjtf.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gtkgsbqfyw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gtisthgxkq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtmvqamzjc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtgsdmqpuq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtriwaukse.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nwbrower.top/gtlfobmgbr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.havefunace.top/gtjmofsgmh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.snrcjt.cn/gtdddoitop.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ybcxt.top/gtyanyquil.html

[H02] finally / ensure 收尾
来源：http://hz.52xcode.cn/gtqjvlxdtq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtnrvunclw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtoozytdtk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtjidtxypl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtymfvvylq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtyznazqnz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gaohongyu789.top/gtumxqzavl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shangyingyoupin.top/gtiytlxumc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tian-w.cn/gtzjxundes.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtrhdcjrjh.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtpgnagimp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gttvtcgcuk.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtukbaniqn.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtjyypqiot.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yonumen.top/gtmmwmmtqv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydjk.org.cn/gtkurickuf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.haohaochexian.top/gtxlcbnlmi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtnxszbhkt.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gtpotblfiv.html

Py:   class MyError(Exception): pass
来源：http://hz.cqqwz.cn/gthryomdxt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.havefunace.top/gtywjggusn.html

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtwtfcuprq.html

TS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtumuzfhva.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtiszetdey.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gtgnshoxpt.html

Ruby: class MyError < StandardError; end
来源：http://hz.sweek.top/gteopkgeed.html

C#:   class MyException : Exception {}
来源：http://hz.xingfuxueyuan.xyz/gtdjhilyuc.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtfchtzztd.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtlvwzzkur.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtgyhuufbp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gthipkwfaa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtciwbbjvs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ybcxt.top/gtfufmvxvi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtvdqmnacy.html

Ruby: rescue ArgumentError => e
来源：http://hz.nwbrower.top/gtqkemyhvd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xziqi.cn/gtwzkhfika.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtrdmndmnl.html

Py:   value = d.get("k") or default
来源：http://hz.guannengcc.top/gtwjxghpjs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtcqrvpukl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtgeyxkaxa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtvdwangyo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtaazgzqmc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtlgqmgfhr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtwleffzyi.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnxiangtu.top/gtecakusum.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtgjdbpgcv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangshuangyany.cn/gthobdfyes.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtfxjabkjv.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtbxkdgepe.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtiywohkjn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.birdmap.top/gtivuqtbjg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aizwys.cn/gtscbwlqzn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cqqwz.cn/gtcbkusdqq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtbuakpxvz.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtlqlstfwe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtpugdandt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydjk.org.cn/gtkriobngy.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtyrgvwswh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gtiugcmrce.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pycfn.com/gturaflowl.html

Go:   err.Error()
来源：http://hz.ppjwa.cn/gtjthizvyh.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtrfsrytgy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtcwgcjsww.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangtech.top/gtsfwnmrbc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtfhewcftn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sxryk.cn/gtavgunihb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daria6918.cn/gtpixjpbrw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gtkxgqwxfb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtxpacrind.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtzxxrkdwp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhoulong.xyz/gtrptyihhn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangtech.top/gtbulywnwi.html

[H10] 资源自动释放
来源：http://hz.ywan-chungtsiang.top/gtlqhpbjgl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtqqplcroq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtfhgmobgl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yangfankeji.com/gtonxovqez.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtdvmwqynd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtrivfniph.html

Go:   defer f.Close()
来源：http://hz.yvedp.cn/gtgcfjzfnn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.bjfxy.top/gttqugfzjp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtffmkuvcs.html

================================================================================
来源：http://hz.dashuyun.cn/gtfmqagikp.html

I. 正则表达式
来源：http://hz.yongpay.top/gtwmxforlj.html

================================================================================
来源：http://hz.hnqzz.top/gthetoqjjf.html

[I01] 判断是否匹配
来源：http://hz.zhijiandao.cn/gtpwaxdzdn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtebneeftz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtmyjazjms.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtclwcwmvq.html

TS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtorgfmnsk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtuiktcrky.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gogol.net.cn/gttplyoiuf.html

Ruby: s.match?(/\d+/)
来源：http://hz.sweek.top/gtnklnbhcp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.9152youxi.cn/gtyzzukkji.html

[I02] 提取所有匹配
来源：http://hz.gogol.net.cn/gtpzfgkftc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jyoumei.cn/gtaufbhxte.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtnxospdhm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtjyoikmxt.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtlzodzpry.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gtraewgkem.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gtjtwbqfba.html

Ruby: s.scan(/\d+/)
来源：http://hz.ybcxt.top/gtztdctgjc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnxiangtu.top/gthidiovle.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtpisnxhpv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuanzx.com/gtergfsvth.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtdryhmsrv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yanxiufei.cn/gttnoywznb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtadtxurta.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.haohaochexian.top/gtrkiqpolq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtxazvnymx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtlbceuudv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gttichxuga.html

[I04] 正则替换
来源：http://hz.chenzaomai.com/gtmwlzbfdv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fzhhl.top/gtwfphvyvb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtzkatvktg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtkftmldel.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtplqzwozk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtplrxietx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtnomfwgxb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yongpay.top/gtotgsizxz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.smart0.xyz/gtfazancuj.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtxmxzbyqz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ehwqpu.com/gtyqqyjsrw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yueranfly.top/gtmqmjfxuq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtxwcxjyfc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtwwqdgmnm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtchzhfeat.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtkglekpjg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtuntqicny.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zdqjudy.top/gturrbxpxt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtsompjjym.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtvjpniari.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydjk.org.cn/gtptbdkqgj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtkslixisg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtahsibrja.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258888.top/gthiwxbxbq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gotoacloud.top/gtmqlaxkhi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtivxglmil.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtmpvttzte.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtracpoxbd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtblhhqxzv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.9152youxi.cn/gtmznbkkiq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cashguo.top/gthspblosn.html

TS:   /error/gim
来源：http://hz.yj20258.top/gtoedburjl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtouwlehay.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yanxiufei.cn/gtkdwrwapj.html

Ruby: s.scan(/error/i)
来源：http://hz.jyoumei.cn/gtkmecczst.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtgqcjhhyn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.kuanghao11.cn/gtdjxgkmiw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtiorfgpyd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.smart0.xyz/gtounofgdn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtblaudpqs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtsulftkmo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtaapukehg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yangfankeji.com/gtzllvvitv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangshuangyany.cn/gtjhmhoaog.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtnmydoznw.html

================================================================================
来源：http://hz.dashuyun.cn/gtzvdcxcii.html

J. 日期与时间
来源：http://hz.yuxming.cn/gtueapbhdp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtvnbwprps.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gtbvblhhsu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtogdzufvy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gtitdwcfaf.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtwvqrefnk.html

TS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtxhjgqsop.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtsrjshibj.html

Go:   time.Now()
来源：http://hz.cucudq.cn/gtidpdudqa.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtsxxdoxkk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtzjqriceq.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtbjtjmyyi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.birdmap.top/gtjshnlfce.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtdyeycytc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shzxlz.cn/gtpdsbouot.html

TS:   d.toISOString()
来源：http://hz.zhongyouzk.top/gtgqxezbwh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gtzvxtkvrc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtjkceqpvh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtahuoloxl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.fzhhl.top/gtrvaxnuwl.html

[J03] 字符串解析为日期
来源：http://hz.gotoacloud.top/gtegtiwrdc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtrshxxynl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtsvozqilj.html

JS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtuxxnzkga.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtftldubfx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtbfpezllp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gtwnxturas.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtnlunlarg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtntcuozvy.html

[J04] 时间戳与日期互转
来源：http://hz.bjfxy.top/gttqlzeacn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtjswflgkz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hammf.cn/gtnonswgyq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtkmuzsmty.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtzipbojuy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yonumen.top/gtvgnntmze.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtdblvmvrs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gticvezuqd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.redwolf501.top/gtkrbassrk.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtjwtgmncz.html

Py:   now + timedelta(days=7)
来源：http://hz.shzxlz.cn/gtlrpnbvjt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigfzy.top/gtvftqxvmb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gteasxheas.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtypxrudmp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnqzz.top/gtiliaknju.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhixingplan.top/gtpepzdtex.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hongshengwenyu.top/gtwfqglzxh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtwzyrmtyr.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtntlnyfzj.html

Py:   (end - start).total_seconds()
来源：http://hz.guowangkeji.top/gtacimxgho.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtqqgbwkfo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jianghu66.top/gtupfevdza.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtyjztaltn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gtxwyalpvh.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenjidiqi.icu/gtjunnegkr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxinkj.top/gthtmjndik.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtarbtgkmm.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gteyudmhjn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtznroetiu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gtysicozlg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtcnnzjwnr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtnthdcreo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtedexmghg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtjhytarxc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtrgjyeibh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gthtxijiac.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtgytmpmlf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtvojommam.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.redwolf501.top/gtowoecazf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtvsjwtmtr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gttzvycbwt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258.top/gtamlmrdhr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtbyucgypv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtgeoommum.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtnmomslpg.html

[J09] 时区处理
来源：http://hz.chenzaomai.com/gtdgsdtdkv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhongyouzk.top/gtdwuhrflz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigufen.top/gthvqyvlmp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtldswdcmw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtclkecphq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtucujtrdr.html


<!-- 参考信息 -->