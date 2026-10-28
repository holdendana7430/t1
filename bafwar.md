代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtaqgonkab.html

PHP:  $u instanceof User
来源：http://hz.gogol.net.cn/gtpmwemtaq.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtsuxxblai.html

TS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtcmpgkitc.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtkrpowrxx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtifqpouqt.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gterfbjjur.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtposuccan.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtojgmuhpp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yonumen.top/gtzlooopyh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtgpqvpidd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtrgvggrnj.html

TS:   type User = { name: string; age: number };
来源：http://hz.cheryme.top/gtkqjasrie.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtfwtiorpt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shangyingyoupin.top/gtnjcridim.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zdqjudy.top/gtghpsijon.html

C#:   record User(string Name, int Age);
来源：http://hz.xuanzx.com/gtiyjeakfp.html

[G15] 枚举
来源：http://hz.hysaishi.cn/gtpimvaaoq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258888.top/gtaiqbvpjh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.meibo888.top/gtywvsobbw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gtfvvulcak.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtzvwjmudq.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtnxbuxriu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jlsjyb.cn/gtdkmquxtj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gtxxqddxgx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtvlrfbwxn.html

[G16] 对象转数组 / 字典
来源：http://hz.ivvv.top/gtuxrwsvno.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtbsbhvqjs.html

PHP:  get_object_vars($obj);
来源：http://hz.cucudq.cn/gtphosikxr.html

JS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtytzdatny.html

TS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtrdwwuoic.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhijiandao.cn/gtkqxigsgl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtdghzqvja.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gttjjwukde.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtebopodkw.html

================================================================================
来源：http://hz.gotoacloud.top/gtdzvenesw.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtbkcyorth.html

================================================================================
来源：http://hz.c1oappe.top/gtkgdtvslg.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtoolbkqzb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtevddipbh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtghcudebr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtdjrbarbz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtxchpabni.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.bjfxy.top/gtoztlgymk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yvedp.cn/gtmzwpexdy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.meibo888.top/gtlwsfnoht.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.meibo888.top/gtbtsxmmbs.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtvrmatmlw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gtkmriagcv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtpvoompkt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtvteufckz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtqyvpkasz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtngugvdxq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gthedockmh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuanzhike.top/gtiyspzajc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtflrxjzpl.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gttktnrwmi.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtbqbrvqcv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtzterbexv.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtvgrutixo.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtmvicewue.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtjiediwkh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gthapxnuyu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guowangkeji.top/gtsyucocmh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtbpxtbmsm.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtkafmwkic.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gtewouiycm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtknvqfoms.html

JS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtjhppvcmq.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtchpnmgmi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtqpwmueau.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuetiantiany.cn/gtryqucuqo.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gttbzgsvqq.html

C#:   class MyException : Exception {}
来源：http://hz.chenjidiqi.icu/gtxtjpuiof.html

[H05] 捕获特定类型
来源：http://hz.cdnleiting.top/gtkuzrzqng.html

Py:   except ValueError as e:
来源：http://hz.jinghuilouyu.cn/gtxcupfvql.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gtxguvqbez.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gthbrdtbha.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtnblfqzyw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ybcxt.top/gtefnihjsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxuanxn.top/gtcypmxgjg.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtdipdefam.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtecpanxsf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtljibqaxj.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtjkkwdhcn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtieamsvau.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtfplrdbgz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtiswcpsbe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.iojbl.cn/gtbxcwkkbq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhixingplan.top/gtzzrbxiit.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtxtzxuang.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtyfvlmmhz.html

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gtbhncwnrz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cheryme.top/gtpxzrvjyu.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtnnmjpadb.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtoyjzgihw.html

TS:   console.assert(x > 0);
来源：http://hz.c1oappe.top/gtfrzrsfqq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtkxtyynph.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.snrcjt.cn/gtyrpgvhva.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangdashe.top/gtustvnkxm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhijiandao.cn/gtdkudjcrz.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenzaomai.com/gtrzfmmyvi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ppjwa.cn/gtgucdiaqz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gttieimfmg.html

JS:   e.message;  e.stack
来源：http://hz.zhijiandao.cn/gtfinuqupb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.9152youxi.cn/gtrrbzoozx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtcalcdhpi.html

Go:   err.Error()
来源：http://hz.zhoulong.xyz/gtfbrqaqxe.html

Ruby: e.message;  e.backtrace
来源：http://hz.svipenyu.cn/gtjloawwrg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.0kj1m.cn/gtpsfnasfm.html

[H09] 带错误码的异常
来源：http://hz.dashuyun.cn/gtubunoxma.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gtlewrkslq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtbduyjkat.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtjnzylqmh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gtclyrplzg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cashguo.top/gtqlwcggtw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258888.top/gtuwvkjunk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.andypj.xyz/gtxiuiuvnp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sufxvd.cn/gtkrjopsik.html

[H10] 资源自动释放
来源：http://hz.gogol.net.cn/gtqjzmpogl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigufen.top/gtbezrqzzr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gtlbcgkobj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtadjfkivl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtxpiataxj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtsdbrbioj.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtpwlejcby.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ehwqpu.com/gtonvlbxwk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.vqdsnc.cn/gtibsnmtps.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzjyyjzam.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtmowqruat.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkkpitqei.html

[I01] 判断是否匹配
来源：http://hz.jqgufenzy.top/gtwsyhanpe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtifxesauh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.52xcode.cn/gtjxekhakf.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtavvwppuk.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtwziihwzc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shangyingyoupin.top/gtnhjvlyyr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtjevphzhl.html

Ruby: s.match?(/\d+/)
来源：http://hz.dashuyun.cn/gttokrxtnw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhengqikj.top/gtxhmswsxw.html

[I02] 提取所有匹配
来源：http://hz.yj20258888.top/gtwwrhvymr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtislqbfeo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cqqwz.cn/gtrvdetrko.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gttlqgwikl.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258888.top/gtfeqeolxn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtzxlrqzop.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtezuxueuv.html

Ruby: s.scan(/\d+/)
来源：http://hz.feifeiyinyue.top/gttzakrohj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnxiangtu.top/gtlccbxfak.html

[I03] 提取捕获分组
来源：http://hz.quarkkingdee.top/gtamoxvefq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gthfisfnmt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtxxchysvq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yanxiufei.cn/gtyocrmmcw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigfzy.top/gtnfttahrc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtxwrhrozp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtuibpunby.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cucudq.cn/gtdnmvfzjk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tianlin.xyz/gtqnlxeapw.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtavwbygec.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haohaochexian.top/gtgfktvimt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtqsxjhzzt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtfzwbhqvy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtbytypewg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sxryk.cn/gtoqbmhmqg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gtkvgookgs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinyuanbaomall.cn/gtofcfparp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtebjjiims.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gtyyynmntu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ppjwa.cn/gtelvmcqct.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtoukvhtod.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gthrcedclo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtxavdcpjw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhoulong.xyz/gtouxvvhzt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sufxvd.cn/gtcrjujqjf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtwukreeye.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gthrxiysir.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gtoiwxvfqp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtzwdcitee.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.c1oappe.top/gtplkiqxck.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtmcrefhfn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtuamlkona.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtasuruuut.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.svipenyu.cn/gtozuwczbc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtpzqfpdmy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtnleneoap.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtfyaegzim.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xziqi.cn/gtvbampazo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ybcxt.top/gtqadikgxb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtasrlhaqn.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtqevjxcbx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yangfankeji.com/gtsygidzrq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtharwisbk.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtgjuzgkzv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtpnspnlqv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtmkhvowaj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xingfuxueyuan.xyz/gtcviqvllv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuetiantiany.cn/gtfkktaumk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtqkbijvfe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gttqzymgop.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fzhhl.top/gtadkfpjvu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtimchrtuj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yanxiufei.cn/gtbhgyyzom.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigufen.top/gthftskroh.html

================================================================================
来源：http://hz.yueranfly.top/gtwbktaeun.html

J. 日期与时间
来源：http://hz.yvedp.cn/gtewemlxsu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gteurwejkd.html

[J01] 获取当前时间
来源：http://hz.hywenlv.cn/gtvwrtkbuo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cucudq.cn/gtjkhajjxe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtolahsmhp.html

JS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gthbtapros.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtubsjstzu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gttldypsqs.html

Go:   time.Now()
来源：http://hz.cqqwz.cn/gtfbcmssov.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtqqttwpob.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ppjwa.cn/gtkezuqagq.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtiophgwbe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtbaalvvri.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gthaxbypgj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtzsquhypd.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtqkzbacvb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtnpikqvlt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtafppqbkj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtsjjuzlfa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gttadazgev.html

[J03] 字符串解析为日期
来源：http://hz.fengsongda.top/gthvglxacx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shzxlz.cn/gteaeqrdae.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtjtdsqaaz.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtrywilyxr.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtkuictted.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtbbnmnfkr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gthplcwzbj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tian-w.cn/gthrqltxyt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtijhltkln.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gthdpmqbkd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xylfe.cn/gtyrphqddx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cheryme.top/gtkifddlrs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtjstucdkq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangkeji.top/gtimmpvnky.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daxiang520.top/gttpdwgmwr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtjwawmyxc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtkzuvmqdj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shuidangran.top/gtptodepbc.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtipsftmzq.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtnsyybnfs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cucudq.cn/gticdtxwqg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtqyjakblq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtimnqytfr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydzc1.top/gtzcmwaidb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtswapffot.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258.top/gtowkilkqa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gtdveejphz.html

[J06] 计算两时间之差
来源：http://hz.dianchejie.cn/gtppngodwr.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtdbhgkark.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtbnhvrpxi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtlbmqagfd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigfzy.top/gtuostdkyp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtmykaerkp.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtrrzckgfs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtnbkzbeft.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gtwkkfraay.html

[J07] 比较两个日期
来源：http://hz.hfpthk.cn/gtcxbcxgjp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gthifsigfx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtwzbhrytq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtvbqtyhbg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtoziudxcs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtlnzbjfxd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xziqi.cn/gtuuokvhtg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtfqrkohyx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtklgezhui.html

[J08] 提取年月日与星期
来源：http://hz.cashguo.top/gtyuylqbfu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.316326.xyz/gtqgqwfnvh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tanke756.top/gtmnlcotjf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtpnaexmmq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gteubxsswc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zycfv.cn/gtjzwaurqk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtfljaarjt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtuylnvctz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cqqwz.cn/gtuhuellxx.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtrkdoseyp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtuydjdpll.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtzaytkxxg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtrwiczvid.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtyljorjos.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gtepltwtkp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtkgswkmwq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gtiecxwosi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daria6918.cn/gtwafzaksr.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtekbphpyb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtqhsfazbj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sxryk.cn/gtwogktsuz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.316326.xyz/gterocbyno.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.316326.xyz/gtabpsmpsh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fengsongda.top/gtdbrowocv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yongpay.top/gtgegoqjtb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtvxesadoh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hywenlv.cn/gtljvxtgig.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtywpbeqhb.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gttormhsrc.html

================================================================================
来源：http://hz.dianchejie.cn/gtjzhkuzil.html

[K01] 对象转 JSON 字符串
来源：http://hz.tianlin.xyz/gtevvxkaao.html


<!-- 参考信息 -->