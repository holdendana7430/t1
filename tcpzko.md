代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtudjlspnb.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtuqbhrdao.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtogxvwfcq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtkogezobr.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gtcihqfvsj.html

C#:   public string Name { get; set; }
来源：http://hz.ybcxt.top/gteulghldd.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtpzadmrxd.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtkqqwznqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtocaovibr.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gttbdgjibo.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtpmlchkgi.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenjidiqi.icu/gtxdygydln.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtwlgbuptj.html

Ruby: def to_s; @name; end
来源：http://hz.zhixingplan.top/gtydjogvlz.html

C#:   public override string ToString() => Name;
来源：http://hz.jiagoushi.top/gtzuxpvsdd.html

[G13] 判断对象类型
来源：http://hz.aibaodan.cn/gtrchwyegw.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtvxeqyzez.html

PHP:  $u instanceof User
来源：http://hz.quarkkingdee.top/gtraddpsao.html

JS:   u instanceof User
来源：http://hz.hnqzz.top/gtmuiqlvzg.html

TS:   u instanceof User
来源：http://hz.yonumen.top/gtcgyueets.html

Java: u instanceof User
来源：http://hz.xylfe.cn/gtfluyucwp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtehduoqur.html

Ruby: u.is_a?(User)
来源：http://hz.zdqjudy.top/gtmkahsaum.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtlvumcyhj.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtlxmztjfe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtzlymeczl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ppjwa.cn/gtdhqqrzcg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtkmabdapt.html

TS:   type User = { name: string; age: number };
来源：http://hz.iojbl.cn/gtudzsqrap.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtvzlkkzkw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shzxlz.cn/gtrgjrstpn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gtxylkxrvd.html

C#:   record User(string Name, int Age);
来源：http://hz.mhx1999.top/gthhmhqpby.html

[G15] 枚举
来源：http://hz.hfpthk.cn/gtclnhwika.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.52xcode.cn/gtkqqqcgdl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtwhkpoijc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtgzlxcwer.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtlkdnycib.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gteyppeuup.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ywan-chungtsiang.top/gtdibplrgv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zdqjudy.top/gtbkwqigao.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtrslmqxnh.html

[G16] 对象转数组 / 字典
来源：http://hz.snrcjt.cn/gtkxelnxgu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sxryk.cn/gtplbesixk.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtnouzibrw.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtcywqunjo.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtcjfejomx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zdqjudy.top/gtzlddcwpi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtvcdvbbno.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtwmvzqbzh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuanzhike.top/gtsgydzbeq.html

================================================================================
来源：http://hz.mhx1999.top/gtixclwigb.html

H. 异常与错误处理
来源：http://hz.tanke756.top/gtpzekwrru.html

================================================================================
来源：http://hz.9152youxi.cn/gtwkhuvfrb.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtopsyeyfs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtnvaoemjv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhoulong.xyz/gtgpubpycy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtdykmdmep.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtpyugezdx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gtqmioorhk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtxuelcjep.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtscdlwunw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258888.top/gtognyuzqd.html

[H02] finally / ensure 收尾
来源：http://hz.yvedp.cn/gtyrkxarkm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtopcsgvmt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtgwdqkbzc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtdembbjle.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gthjtvovjn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtddmfubty.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gtcgsosesu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtwinbxrjs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xinyue.icu/gtsrslibwx.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtztjhmqku.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtxngbbdpl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtymmgzwmc.html

JS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtmgtkicqi.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtszdxbkbh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtmznmincw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtbspbjfns.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cheryme.top/gtnsohvjob.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtkwzrlbfb.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtihmmjlnx.html

Py:   class MyError(Exception): pass
来源：http://hz.pengpengdd.cyou/gtastqjxem.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtsojseuha.html

JS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtdjdnalif.html

TS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtkvbtsqzo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gttpssvttg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hysaishi.cn/gtblylwubj.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangkeji.top/gtaythpour.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtqblorgdu.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gtutptwnry.html

Py:   except ValueError as e:
来源：http://hz.cqqwz.cn/gtezlesrlk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtihbrlagj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtdxwprzuy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtwunnhxyt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuanzx.com/gthlpumsej.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtzqqhelyq.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtsauqfwkt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtdonzmkft.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gtjfurswas.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gthkqjoqxv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtpukinyam.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtmkfsvbqd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtqyjnpmnd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258.top/gthsjldwyn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtresngelo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hongshengwenyu.top/gtkzufziya.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtqebfumhd.html

[H07] 断言
来源：http://hz.kuanghao11.cn/gtcigvotmt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cucudq.cn/gtlpebruwk.html

PHP:  assert($x > 0);
来源：http://hz.nanxuanxn.top/gtooxsdfel.html

JS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtihpwoiae.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtexatzzqv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gthamqlihi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gtjmczgsuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yueranfly.top/gtftmvpsne.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtyzqzqejm.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtoxpjesad.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtwhbmxtay.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.vqdsnc.cn/gtzdsrdato.html

JS:   e.message;  e.stack
来源：http://hz.vqdsnc.cn/gtepfzzemn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtbxqxjgjt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtxyuxgdnl.html

Go:   err.Error()
来源：http://hz.sufxvd.cn/gtlgrtjwgg.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtnfwzgwct.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtgphcqhwl.html

[H09] 带错误码的异常
来源：http://hz.hongshengwenyu.top/gttdvyjfkz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gtivexjaoe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtdquqwhto.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtyzgskini.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ywan-chungtsiang.top/gtjavwzxdi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yangfankeji.com/gtuuvklmff.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xylfe.cn/gttfsdatkd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtqthxqpre.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigufen.top/gtpcegzmby.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtehjvxwij.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gtngiaaktm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtxpirfcfx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtplfarnga.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gtqyvwnldb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtmokzecjk.html

Go:   defer f.Close()
来源：http://hz.fzhhl.top/gtlpcfvnhj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.quarkkingdee.top/gtfydjoaes.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.mhx1999.top/gtjqcqygel.html

================================================================================
来源：http://hz.guowangkeji.top/gtlpmjdicd.html

I. 正则表达式
来源：http://hz.yj202588.top/gtqlgoldmt.html

================================================================================
来源：http://hz.ppjwa.cn/gtkveyjhda.html

[I01] 判断是否匹配
来源：http://hz.yvedp.cn/gtwbewvqmq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daxiang520.top/gtnohpngfd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gttalstske.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtpqzeueyg.html

TS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtugkxvlnd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shzxlz.cn/gthsfjtnmg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgufenzy.top/gtridtdidj.html

Ruby: s.match?(/\d+/)
来源：http://hz.kuanghao11.cn/gtsfxistut.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtuyyhbpub.html

[I02] 提取所有匹配
来源：http://hz.316326.xyz/gtjlmqnaqo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuanzhike.top/gtmwqzrdlq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cqqwz.cn/gtuscwmkmj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gtusrmnloh.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtiynrvxrt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yvedp.cn/gtrwdfrvxw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtiwirhcao.html

Ruby: s.scan(/\d+/)
来源：http://hz.ehwqpu.com/gtzbydtdxc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydzc1.top/gtzfpcaaop.html

[I03] 提取捕获分组
来源：http://hz.shzxlz.cn/gtkfaibxfn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gteilrpcoq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtlbxhheoi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.feifeiyinyue.top/gttvgrrquk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daxiang520.top/gtamlwzzov.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangtech.top/gtthtwyfwp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhiwuduotai.top/gtbzfwpasq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jiagoushi.top/gtdjiefnxm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ivvv.top/gtysvesdqe.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtqgwgybut.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtruolpyiq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtnbphupzi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtldsiiiru.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtaybmmadb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.c1oappe.top/gtwxetbjof.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gtmlgdrbnn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtoaqpxjix.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtnaarhyvs.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtmtftqpdw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gtqurtibei.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.haohaochexian.top/gtnxgrpbot.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtqktchzkr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtiscjfspr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guannengcc.top/gtmiwmsnvx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gtfdwetrul.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtxacnkhuz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtieelzzob.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydjk.org.cn/gtsquwohfh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxuanxn.top/gtclasoqlf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydjk.org.cn/gtklmgtjqu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtzyuevoex.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtfdivqlxo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gthnhvhqnx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhijiandao.cn/gtmirlgkig.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtgmzdfijv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtvslbgszc.html

[I07] 忽略大小写与多行模式
来源：http://hz.pycfn.com/gthawouehq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.quarkkingdee.top/gtxhbjfdny.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtjltwzsih.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtzosdugre.html

TS:   /error/gim
来源：http://hz.nanxinkj.top/gtmqtlvduj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtttfggpum.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnqzz.top/gtwxzqqxti.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtjmzvbxst.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtmorkxmvg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtookewiyy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhengqikj.top/gtekeswelz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtomskxmey.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtrghujrfk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gtjvvcayde.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sxryk.cn/gtvtnsncay.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.snrcjt.cn/gtcmecshdm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gtqbecfqge.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtfxgypluc.html

================================================================================
来源：http://hz.cdnleiting.top/gtbjazvttb.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtxvtkvmbx.html

================================================================================
来源：http://hz.nanxuanxn.top/gtzugvovzv.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gtkgdjpefw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtehnzilmy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtjehjwpum.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtifdfxrnz.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtecgjsizg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.c1oappe.top/gtbhjxgwnk.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtkbkmcedo.html

Ruby: Time.now
来源：http://hz.gaohongyu789.top/gtxwprjggf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sxryk.cn/gtejwkkebh.html

[J02] 格式化输出
来源：http://hz.316326.xyz/gtuttznewe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtoipvxrlv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.mhx1999.top/gttamhmwpp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtesigameq.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtjeqyguim.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gttdqcxwwp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zycfv.cn/gtfqocoyew.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtypzwzvoh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gttwwxgobz.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtxflkkdjx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtefifxuts.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtesouwpsk.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtintinuta.html

TS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtpfmqjcsk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtrkcelwxb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhiwuduotai.top/gtcazyuchm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtezlqmyrk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtxlczfvse.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtjulojaoe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtatxketsp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtrpwrtfem.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.9152youxi.cn/gtsmdbdtbo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hywenlv.cn/gtgwzwqqha.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtfmgzxtyx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.snrcjt.cn/gtoghdhhvs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtorfttimz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinghuilouyu.cn/gtuzaohioz.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtsbbixzwy.html

Py:   now + timedelta(days=7)
来源：http://hz.tian-w.cn/gtvxnulmkw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtzjgwqcua.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtvtusgmaj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtjuzxedgv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangdashe.top/gtewslfbvy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gtgpfqbhhk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fzhhl.top/gtwbnhthxy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtsvmtafpn.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtdkvwkmpv.html

Py:   (end - start).total_seconds()
来源：http://hz.chenlongwang.top/gtnsutjqsa.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtaqsalcxr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258.top/gtuttcqkpj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tanke756.top/gtrqewhgss.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.haohaochexian.top/gtiniixtca.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtrcozlvoy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.c1oappe.top/gtskmbbnxb.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtfpvtymzx.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtiueazlon.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtewrkhupj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtkvubkuor.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtfkflmobh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtklqfbyko.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtbvsozcam.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuanzhike.top/gtmwoluhhx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtxyuikabp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gthuxacpur.html

[J08] 提取年月日与星期
来源：http://hz.feifeiyinyue.top/gtjusbicao.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangshuangyany.cn/gtinjwkxtq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ybcxt.top/gtryudxewq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxinkj.top/gtljynanyl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.bjfxy.top/gtoygedhsd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtpjtupmra.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guannengcc.top/gtoegwelnb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtlvhmabzy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.kuanghao11.cn/gtubimqbtb.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtwhpuebvw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtxhckixcy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtgcreerbu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtgpfdrkgs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtqoxeaacn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gthdjmenas.html


<!-- 参考信息 -->