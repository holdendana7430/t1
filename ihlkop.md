代发 wailian999

[G10] 访问控制
来源：http://hz.ydzc1.top/gtfurmmjwk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fengsongda.top/gtvphzwebv.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtvsmklmlq.html

JS:   #private 字段；其余公开
来源：http://hz.chenzaomai.com/gtzwkrcreq.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtlnzjyzoi.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtrtyghcgx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtwwqhduuq.html

Ruby: public / protected / private
来源：http://hz.gotoacloud.top/gtxhvjybui.html

C#:   public / protected / private / internal
来源：http://hz.gaohongyu789.top/gtvnvqtfur.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gtihkxvvpv.html

Py:   @property 与 @x.setter
来源：http://hz.havefunace.top/gtclwduzgz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtdnewgact.html

JS:   get name() { return this._name; }
来源：http://hz.sxryk.cn/gtzcastpqz.html

TS:   get name(): string { return this._name; }
来源：http://hz.hongshengwenyu.top/gtemjvqgmd.html

Java: public String getName() { return name; }
来源：http://hz.xuetiantiany.cn/gtxesdfbee.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtvqsmlewh.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtmobegehf.html

C#:   public string Name { get; set; }
来源：http://hz.sweek.top/gthahoihsy.html

[G12] 对象转字符串
来源：http://hz.chenlongwang.top/gtectcuywv.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gthsjndnmx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtohaaytuc.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtdruyugsh.html

TS:   toString(): string { return this.name; }
来源：http://hz.daria6918.cn/gtckjejggv.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtkwcposgb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtpsfagcmf.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtltombxpi.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtdhhjlapc.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtvgvuzelw.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gteaarrgum.html

PHP:  $u instanceof User
来源：http://hz.haohaochexian.top/gtqrrrwikz.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gttuhfwxqg.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtgroxaemi.html

Java: u instanceof User
来源：http://hz.sysykeji.top/gtonyaezri.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gtyqfzopfz.html

Ruby: u.is_a?(User)
来源：http://hz.gotoacloud.top/gtojpvzknk.html

C#:   u is User
来源：http://hz.yueranfly.top/gtuthcwfvr.html

[G14] 数据类 / record
来源：http://hz.yuxming.cn/gtorxnuoxx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guannengcc.top/gtksozllgo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtebhvslhb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtjqutiwax.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gtpfxqfazh.html

Java: record User(String name, int age) {}
来源：http://hz.yongpay.top/gtnnqprxdv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtpjekkjfm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gtavygybkq.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtiqizstnl.html

[G15] 枚举
来源：http://hz.wangdashe.top/gtoqvuhzhz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtaqcrvwcf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yvedp.cn/gtsujipbtz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxuanxn.top/gtjfkkeron.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtphnitzqe.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtguzozewd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtjfewvkgy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtzsdpfmsv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtayzgfgwa.html

[G16] 对象转数组 / 字典
来源：http://hz.xuetiantiany.cn/gtpystieky.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtpukaafvd.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangtech.top/gtlnwvxurq.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtnjzlndzk.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtkqbfzdrq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtczjqbvaj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jyoumei.cn/gtkflffrhz.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gthgtimchp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gthjxuckoc.html

================================================================================
来源：http://hz.fengsongda.top/gtuipfqtxo.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtyujnauvu.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxdjwccdv.html

[H01] try / catch 基础
来源：http://hz.hnxiangtu.top/gtozybvksl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daxiang520.top/gtidzfnqic.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuetiantiany.cn/gtalrunqdu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtrbntsdiu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fzhhl.top/gtxnjbfzle.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtbkvmbtaw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtzppiblkp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gtdrxqvlfb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yongpay.top/gtmkvecubm.html

[H02] finally / ensure 收尾
来源：http://hz.jinghuilouyu.cn/gtuliumvot.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xinyue.icu/gtzofhegcq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtjvkhkudn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtkvuqjjze.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtvdvowokb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtdrvodjym.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gtdjtjjmhq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtnefpibdg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydzc1.top/gtsugaygnh.html

[H03] 主动抛出异常
来源：http://hz.jiagoushi.top/gtgxpnkvkg.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangkeji.top/gtftojdxvg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtunvoxjtt.html

JS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gttarjixpe.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtesfnqyqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtzrexhlbo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cashguo.top/gtqrfbkcth.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtibcmlpbo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtjgjzauve.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtyjiofehy.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtweascuqs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtbxqdqutq.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtfcqofdgj.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtilnxefmk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ybcxt.top/gtjfbpnoka.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jyoumei.cn/gtdtxlgyft.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtmvbgpser.html

C#:   class MyException : Exception {}
来源：http://hz.jqgfzy.top/gttkftyejt.html

[H05] 捕获特定类型
来源：http://hz.pycfn.com/gttxndrzts.html

Py:   except ValueError as e:
来源：http://hz.cashguo.top/gtkrjgnftp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtxxhcqwln.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gttmoyouqn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtnmcmfkdl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtkbhihavo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtcolbkbfx.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtwqdcpeof.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guannengcc.top/gtcnubolpg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shzxlz.cn/gtsxdvkkdf.html

Py:   value = d.get("k") or default
来源：http://hz.hongshengwenyu.top/gtysiilyae.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj202588.top/gtxtzhuxwb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtztxnessk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtiyvnuyxd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtpluuqcrv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gtcynrxzgn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtfsagvhpg.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtzgsxqgwl.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtdqvgqgyr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtkxaljqpe.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtsczqcvqx.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtbbnzpgsj.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtdqkmfucb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtxrhcowes.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hysaishi.cn/gtggrsmanf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtsoahwdjz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gtvzqfngle.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgufenzy.top/gtfwrzvjro.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.quarkkingdee.top/gtoucjpchv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtrlkijuls.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtmpbjijdm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtopxfwtil.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gtigpfcufa.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtizdflnqj.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtnkocxdva.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gthrwkrhyi.html

[H09] 带错误码的异常
来源：http://hz.birdmap.top/gtcidxdypx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fengsongda.top/gttroxpzlq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tian-w.cn/gtzcqporuj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gtossvnjzz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sxryk.cn/gtmoskotgh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gthzhfuyvz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtvzzcpnip.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtzpsykzyi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtsrzjrcnu.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtzfzlsbtn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtwhnumoyj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtlxlkeebu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtcbwjtycb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtafyngdqn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnqzz.top/gtlikrmdpt.html

Go:   defer f.Close()
来源：http://hz.ppjwa.cn/gtxtnxtvuy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yueranfly.top/gtahxhfwht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtxndasyru.html

================================================================================
来源：http://hz.yuxming.cn/gthcbcrtyl.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtgjbksczs.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqgkqqykf.html

[I01] 判断是否匹配
来源：http://hz.ydzc1.top/gtnpqvvznt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sxryk.cn/gtckcynlyw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sxryk.cn/gttdhniivb.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtcxkrfmqt.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtyakmjppx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gtndhcmabc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtdxnjppok.html

Ruby: s.match?(/\d+/)
来源：http://hz.sysykeji.top/gtgfsdxsij.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.haohaochexian.top/gtdknlnuvw.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gtemlyxhhq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.birdmap.top/gtyhblajft.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtoygkbdlu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtlxfqaxnb.html

TS:   s.match(/\d+/g)
来源：http://hz.havefunace.top/gthtewcnjk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.snrcjt.cn/gtamtbjgrb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jlsjyb.cn/gtzohjuydt.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtgwnbdtqe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gthkjtpjzt.html

[I03] 提取捕获分组
来源：http://hz.yangfankeji.com/gtvuwyrxov.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangshuangyany.cn/gtdjjupxih.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtudugqqsu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hywenlv.cn/gtckymvztm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xylfe.cn/gtwyjrjbxp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhijiandao.cn/gthzznqglf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtppgbjrnw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dashuyun.cn/gtlqkcueiu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtklczankc.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtcyhtxedc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuetiantiany.cn/gtieailkis.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtczkahiwj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtvicoxjrf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtbvnmbyyr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtmnobvphn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuxming.cn/gtmvswvdtx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtfcojrany.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gtnklgmowj.html

[I05] 按正则拆分
来源：http://hz.zhoulong.xyz/gtbhrszebm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhengqikj.top/gttsvdkrst.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtcjrspawd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtxeweliwr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtfonacnww.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gtjosxcjkz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtujgawtqr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtwynrssek.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtwpojttzd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtaifjlmlc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtnquxliad.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtmymxeasg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtzdywdzsn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtuhdpunml.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtxekwaahs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gtshaboqlx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuxming.cn/gtvshxmiya.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtkmkvluex.html

[I07] 忽略大小写与多行模式
来源：http://hz.pycfn.com/gtpncjolhz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtbqbchtna.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gtoipegnyb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hfpthk.cn/gtsfuncvgg.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtrrpunjku.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gtbiytqmkl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zdqjudy.top/gtobweuhtr.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtjnmjtxwm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtdqukqmlu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.c1oappe.top/gtcwmmukno.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ehwqpu.com/gtvckawbpe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtddirknov.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtcqnchtpq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtofknvifi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtrlwquabt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtgxewbuci.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangshuangyany.cn/gtepzehiss.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtypjruwgv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqbxdcvnq.html

J. 日期与时间
来源：http://hz.zdqjudy.top/gtdxbtuqnd.html

================================================================================
来源：http://hz.hysaishi.cn/gthcsnuljv.html

[J01] 获取当前时间
来源：http://hz.quarkkingdee.top/gtjtoskkls.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtmvupwbes.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtbeuytxbh.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtsgvcveto.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtnmvfkpqu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtroekuggy.html

Go:   time.Now()
来源：http://hz.zdqjudy.top/gtaoehajjp.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtzdaaciuw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtkjjszecb.html

[J02] 格式化输出
来源：http://hz.jinyuanbaomall.cn/gtigvkuanr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtcfdzeksu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cucudq.cn/gtoudqapjh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhaomingkeji.xyz/gtsxcyfrcs.html

TS:   d.toISOString()
来源：http://hz.yj202588.top/gtypvrnhvq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtrzishnrw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtzmnshixf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtniijomyj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtowushvpu.html

[J03] 字符串解析为日期
来源：http://hz.snrcjt.cn/gtalincsbz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtulvffcxx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tanke756.top/gtpigykrqn.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtcxbbjglp.html

TS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtzrvylamx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtrwqdxtfh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gogol.net.cn/gthvaqsolt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tanke756.top/gtsakowzfy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gtriytnpfo.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtvzvrufsy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aibaodan.cn/gtigvotsno.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtsmnkvzpo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtnqmvkmpr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ybcxt.top/gthvtjivix.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gthsktwsfd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenlongwang.top/gtcnvczphi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtqykmjrab.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xziqi.cn/gtivaaiqij.html

[J05] 时间加减（加 7 天）
来源：http://hz.xinyue.icu/gtlpqcuwga.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtlwxtqris.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gteksxdvbt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtdicpabft.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtedrrshuw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.c1oappe.top/gttcbsafng.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gttaznxyec.html

Ruby: Time.now + 7 * 86400
来源：http://hz.kuanghao11.cn/gtemzmeoep.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtywcgqxox.html

[J06] 计算两时间之差
来源：http://hz.cucudq.cn/gtwgqbmwdn.html

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gtkqqhqnla.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtrxwexhlu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtutlrwrkg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtptptwdig.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hysaishi.cn/gtsfjxnltf.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtnnpxngyx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gtfszafafq.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtzgqjyvvr.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtjbcnjphk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtbbitrojh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gtzfckqhpr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtizgdjahv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtwoqnqdtu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtngrmzldd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtndhzkllt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtqncaxidt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtijbdsftz.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gtooxoauwh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gttzdmcakh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenjidiqi.icu/gtfcwenziz.html


<!-- 参考信息 -->