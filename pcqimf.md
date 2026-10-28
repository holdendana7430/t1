代发 wailian999

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtasktzavz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtfvgjhxos.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tianlin.xyz/gtpsnxvmzk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gtrhcyafeh.html

TS:   type User = { name: string; age: number };
来源：http://hz.aizwys.cn/gtefhjpien.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtictjmkoa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zycfv.cn/gtcnnifwpw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtjgytdmek.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtauvlzjor.html

[G15] 枚举
来源：http://hz.sysykeji.top/gtrlqaqjci.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sweek.top/gtllacumon.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ivvv.top/gthzwlujdu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtbhzicchk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtdrivksmc.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gttcrgtdhh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.meibo888.top/gtaxzqrhsa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtoogmgiuc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtweczfpui.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtjmjuuelw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtomebfgpt.html

PHP:  get_object_vars($obj);
来源：http://hz.gogol.net.cn/gtsqwuuais.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtpqfzyiig.html

TS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtxuifmupy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gtctcgvqxu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtwglyiwbb.html

Ruby: obj.instance_variables
来源：http://hz.vqdsnc.cn/gtjdqsumtd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtytxfomai.html

================================================================================
来源：http://hz.yuxming.cn/gtdvrudwch.html

H. 异常与错误处理
来源：http://hz.chenjidiqi.icu/gtpkfgnjzz.html

================================================================================
来源：http://hz.cdnleiting.top/gtwolhuqvb.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtddeffkok.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtbepkvnxk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yongpay.top/gtboqygyob.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtyxliobcx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.316326.xyz/gtkyaugbkx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.0kj1m.cn/gtzuwfnltw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtbyedefva.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gthkarimbh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtcxceynid.html

[H02] finally / ensure 收尾
来源：http://hz.9152youxi.cn/gtgecchzrn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtujnmarjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtutadiokl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtwxbusehj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gttkttubvv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtazpjilgs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtapvivkxq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.kuanghao11.cn/gtsfxnnemf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtrihjneuc.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtyhjzkufs.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtgrepkhzr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtbcgqqziy.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtrhowtikw.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtetrlibrw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258.top/gtzimwgnli.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gtcmqufawu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sxryk.cn/gthfkxfzbd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtlghiogyz.html

[H04] 自定义异常类型
来源：http://hz.yangfankeji.com/gtzpgugahb.html

Py:   class MyError(Exception): pass
来源：http://hz.cheryme.top/gtakinbqcx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtzmcgdriq.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtyfqcoqgj.html

TS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtlmdscxug.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtnokmmkex.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.haohaochexian.top/gtsmviksyy.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtxdabcqzh.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtimbfmwlt.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtdnaaglyb.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtztijzqia.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gtxfbubfrd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtpacbiydn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtduzwsvnd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gteuiyrods.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gzhubu.top/gtpiawpwlj.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtqepnzati.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.c1oappe.top/gtyqzedmhd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cheryme.top/gtsisotglc.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gtbjvuxsne.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhixingplan.top/gtcfubgfhx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtjkzccfhq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtchxwprjf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sxryk.cn/gtssxnwtvi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gtcdptimjx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gtjablidtb.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtkrggpxuw.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtyudsqyjv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sysykeji.top/gtpgigokid.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtxecuurvf.html

JS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtrlqppsxt.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtunamxbzw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtxrrmmoip.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gtmrronwkj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtycsnhkpy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tianlin.xyz/gtqymgesxh.html

[H08] 获取错误信息与堆栈
来源：http://hz.jiagoushi.top/gtxelclobo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtusxyjpko.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgfzy.top/gteylwtgde.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gtwktmockq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zdqjudy.top/gtstdworos.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtyjesogzq.html

Go:   err.Error()
来源：http://hz.xylfe.cn/gtbqimzxzr.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangtech.top/gtzzcbivww.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgfzy.top/gtbmowfztq.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtxheizvxn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gtfpuhlrgz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtinirsosd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yanxiufei.cn/gtuksmgbrm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtwppmcgsi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtzlydcftk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jiagoushi.top/gtuzzmanxo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.meibo888.top/gtzeqnuptm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtvabngotm.html

[H10] 资源自动释放
来源：http://hz.haohaochexian.top/gthejsigra.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gthgefungu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gtfhulwfeb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtugpdeqvx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtywyrhwbq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.meibo888.top/gticqnhqgo.html

Go:   defer f.Close()
来源：http://hz.pengpengdd.cyou/gtumcnuxkx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxuanxn.top/gtsakrotcr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxinkj.top/gtlluginod.html

================================================================================
来源：http://hz.jianghu66.top/gtqoiybzpv.html

I. 正则表达式
来源：http://hz.hammf.cn/gtffevxzru.html

================================================================================
来源：http://hz.ydjk.org.cn/gtaamoqtcc.html

[I01] 判断是否匹配
来源：http://hz.hysaishi.cn/gttnxhgaxn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gtfcxwescm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gtrciizgep.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtdyowqhhl.html

TS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtzlulnozg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.feifeiyinyue.top/gtqwbgdsgp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gtxsmxpxup.html

Ruby: s.match?(/\d+/)
来源：http://hz.cqqwz.cn/gtermwnpdr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gtpfuezymv.html

[I02] 提取所有匹配
来源：http://hz.jinyuanbaomall.cn/gtlrfvtpvj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhengqikj.top/gtsjdlkftn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.feifeiyinyue.top/gtlvuublax.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtejbwgbae.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtkgnjzgbq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.snrcjt.cn/gtbbmkggrx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gtjelmrtsy.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgufenzy.top/gttfjdrtyd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fengsongda.top/gtulgpuebq.html

[I03] 提取捕获分组
来源：http://hz.xingfuxueyuan.xyz/gtlleoiddx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtxisxqkrp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnqzz.top/gtlfzptbso.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gtxofjslvr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jlsjyb.cn/gtelzlseja.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.vqdsnc.cn/gtjlrievfk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jyoumei.cn/gtldjiuerf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtvgoxmipf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dashuyun.cn/gtjcffgbox.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gtmozwmlhq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinghuilouyu.cn/gtggctcnwf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtxxlpkdcq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.c1oappe.top/gtobliklhm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtbaywwxml.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuxming.cn/gtsqrqevlf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gtuhypmcmu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yangfankeji.com/gtsyzntini.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yanxiufei.cn/gtjrmgkhcj.html

[I05] 按正则拆分
来源：http://hz.yongpay.top/gtgqqigymk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhijiandao.cn/gthvququmf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydjk.org.cn/gtqkbwttbw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtqipkdugb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtpgheyeji.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daria6918.cn/gtgdspjyji.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.bjfxy.top/gtluuhaqjx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtjhoigdik.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtdremimyt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtukffrrjs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtdvophdyb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtyppkgmup.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtiztihdib.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtjwohucpt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtabevtvcu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtyxbvoorq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xylfe.cn/gtkhppfpmp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtrosspdvd.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtqbjcgsxt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gzhubu.top/gtrbqsbzvs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtmihomfas.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtlgugeypv.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtalgylrqf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtjvcrbldc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yanxiufei.cn/gtopuqhawr.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtcunzndkl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtzwqqoajz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.svipenyu.cn/gtjrehayxn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtwyotuwpm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtgrqmzeze.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtnsgefbkb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtdhmnntxx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtqdggtgvt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fengsongda.top/gtjiyytpkq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sysykeji.top/gtlchlijmx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtekgwudoq.html

================================================================================
来源：http://hz.sufxvd.cn/gtovwvpoqy.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gtvjafbjba.html

================================================================================
来源：http://hz.pycfn.com/gtnnlvjrnm.html

[J01] 获取当前时间
来源：http://hz.fzhhl.top/gtppftuxmf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtqzfrllya.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtdjnblovj.html

JS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtpcjuimzp.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtcnifkdar.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.havefunace.top/gtxoukzuui.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtycdlwucz.html

Ruby: Time.now
来源：http://hz.zhongyouzk.top/gttchzgpxt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxuanxn.top/gtmqkdcfed.html

[J02] 格式化输出
来源：http://hz.birdmap.top/gtbyeclkks.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtgvdsdxhx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtwtayzfqv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gtgtuhurwg.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtjzlxwkxi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtncvinppq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhixingplan.top/gtqkauixyx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtuifreaml.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gthogufpxe.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gtaicuhhts.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtimunfulz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydzc1.top/gtxnvasxhv.html

JS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtjrqjunmi.html

TS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtmyfzllpu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtqfqldxkp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ppjwa.cn/gtgktcjyda.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtnigrodcg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhoulong.xyz/gtzujszvwh.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gtspdngnvy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtxhxozjcm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tanke756.top/gtpheaudfb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtyuvtwqmc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xziqi.cn/gtvttmlrjt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtmesxhuuu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtymwukbnq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gttefgsmom.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtvizsndrb.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gtsuqesjef.html

Py:   now + timedelta(days=7)
来源：http://hz.zhoulong.xyz/gtuokwftrm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tanke756.top/gtesdkhxze.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtpdomexja.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtgtidapio.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtpaopghim.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shangyingyoupin.top/gtguqjgnwv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtibnrjvcp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gtiweibqvk.html

[J06] 计算两时间之差
来源：http://hz.sxryk.cn/gtfecmfnkp.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtudqzdvzr.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gterlnntta.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtyzoocqfr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gtldibtkfp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtdcoztyll.html

Go:   end.Sub(start).Hours()
来源：http://hz.cashguo.top/gtqzzssfvf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hammf.cn/gtxwvrlvwp.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gteboeviln.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtxxwclrym.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtycfgfvyb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtvurtsymz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtgpqzsugl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtdigjtwlf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtdlzhaoch.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuanzx.com/gtmmzrqjpd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtnmiyhoui.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtsbihcsou.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtvvxmgsfb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydjk.org.cn/gtmdzhncmi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtllmrekdd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gtzoaqntbx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gtbgmgqeaz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtjcgeicvr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtvcjjiugz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gogol.net.cn/gtcwlnumle.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtzplaasfb.html

[J09] 时区处理
来源：http://hz.yonumen.top/gtgexlrcew.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.0kj1m.cn/gthlwrrtlq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtjvrcwibl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtlniszgqt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtpglwnpzd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtwpcbrapt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ehwqpu.com/gtnrwashyb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yangfankeji.com/gtfbfueacp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtpomkgryl.html

[J10] 取今天 / 本月第一天
来源：http://hz.zycfv.cn/gtiytmlbvq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtfzvduvql.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sysykeji.top/gtvmzsecip.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fengsongda.top/gtsmvhxonw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhixingplan.top/gtlwvzzmyh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhijiandao.cn/gtjzpqecwo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.haohaochexian.top/gtxrbfugcc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtpkpjedye.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtdnzwlsrr.html

================================================================================
来源：http://hz.sysykeji.top/gtvxoznoyw.html

K. JSON 与序列化
来源：http://hz.xylfe.cn/gtuervgtdb.html

================================================================================
来源：http://hz.birdmap.top/gtdpohaxpa.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtwjswjhmo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtiwjhyxys.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gthgkjprxp.html

JS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gttcxpnlfy.html

TS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtykjsvorh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dianchejie.cn/gtcprqbjfz.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gttqarqyto.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtgytfcrgz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhixingplan.top/gtdevshidk.html


<!-- 参考信息 -->