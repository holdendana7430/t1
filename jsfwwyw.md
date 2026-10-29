代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gvdwasnii.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gqikhlpce.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gvsfjifku.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gvorlagee.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyaraehur.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gshwfxmwu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzfpsagug.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gofthksbw.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gogcpawvo.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gelppfchl.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gyryplybn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/ghkstjveh.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gwwbooojx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gnodzbyig.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gkmdzhmyl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gajxwiszk.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gcwvrnlgw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gjzjfvtww.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/godpchrwp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gqrtegrhx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gtvhwwjyw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gyuxpoimz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gxizsuzhn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gofzsuayg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gjhtazkag.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gceqrvwfp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gwgesozjw.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gjwvqhvkb.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grxznakuo.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gunamvaqb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gbkxfqcyh.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/ggrmgflpd.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gammyozuv.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gnyzamuba.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/ggdthlxmh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gnzzzvkqn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/glymxcrfq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gvmqeagwb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gsahbkcou.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/ghgzmhqvt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gcwllehpr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gobifflor.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gaessdxpd.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/glgjjikba.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gnoukwhcw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gzjywymdl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gafavxdrg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gylglsvoh.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gsbvwntws.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gwnhtczxb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gpmrmvrci.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gspoopcqp.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gmnfostwj.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gqbhkuudh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/glgwcewbr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gcdcyjojt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gdkxgdwgy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/gngqwpwir.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gbhpnwlsf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gpxwzkqdh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gnoxkjkjp.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/ggzguezil.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gwcszrpgk.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gzsicomrf.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/glzbnhxkt.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/glikrufrr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gpohrdbpw.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gesietlot.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gjvheayhh.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gzigmpbtk.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gsntvtdow.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/grcgxbtgj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gddnrdhkf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gldbtqfvx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/giwgmfccp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gvhrohfrp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gnlqyztst.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gvtepvjqx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gumyakbkc.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gaepqglxn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/guxukcsno.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggmugqaeb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/glkelqanb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/guumjyris.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/guxwzpazp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gslshxzeg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gljkpvdma.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjptduscd.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvvpxyo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/glxddxofb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gultzkyil.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gkilkltdb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gvgziszer.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gqnhcddsr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gzjmxoojh.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gtedimwvx.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gtfjjlldr.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gqfmyhgtm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gupghcgqt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gcclpbkaf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gpojdzmmo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gwchdrjzd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gcumwrvuu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gbdeigobj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gjiiithot.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/goeubqidx.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gdezkfgdi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gfticdjbe.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gurjrfrje.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gtnauepxg.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/ghwykmdde.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gzmhkbrub.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/giythnnmb.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/ghxyktttc.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gkkycizto.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gqklmahuf.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gbrrbxppi.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gyryoxphi.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gevhwnphk.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gkndjvzbr.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gvhuauxde.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gxozzhdvf.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gvudwhhcr.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gbidpvbod.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/giqsabklu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/grdqkrhar.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gtdhurmib.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/glitmxbhv.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gyqeudmyh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/ggivtmtaz.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ghrbfltcc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/grtktqley.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/ghtvvqisg.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gkqcqjvzo.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gnwnhwgxv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gbybdfkey.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gjnhkbtij.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gxwwdocic.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gjfnffkap.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gsivfqpgz.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gzipupugk.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gynzjvwxx.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gtcqmylxf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gmkapiavj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gnuybcluz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gmbburcxk.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/glruxooau.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gbibrhyzj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gbdcggddn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/gruwknsuo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.hesvh.cn/Article/details/gxkbowzuw.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gbsgbuhac.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gqrzswcxw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gzkwljmva.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gvdwnrdxk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/grkdqjeyu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/grfybehww.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gjdpnczsv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gdlkeling.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gxgbcwehn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/gavprtxhh.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/grhffiwdx.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gtavmmbic.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gqstnohml.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/guaqewrqp.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/giygqxwhr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gutpbhuoo.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gjnyrfnbw.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/gpjmuvbhu.sHtML

[A19] 交换两个变量
来源：http://mobile.hesvh.cn/Article/details/guxlzoofi.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/ghktcnshm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/gjbfovhor.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gawixzkqr.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/ghrzfrwwa.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.zdbjq.cn/Article/details/gwkgsblxg.sHtML

Go:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gxmbevvnj.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gvrwolzbg.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.hesvh.cn/Article/details/gsziwlxqz.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/ggyhvtaid.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gosespvhh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/gchjcrbvi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.hesvh.cn/Article/details/gfspbblap.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/ghdzdfksv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gmqpuuybh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gipdtidbd.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/granzeiwn.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/gcxfvzpsy.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gbdwrarin.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gptsvrsxf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gkkccgubr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gzfyodiwm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gbvgotnel.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gbyxpiyzv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gfdkplpss.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/ghzukmaeo.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/glcvyjwmj.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gkwhyetwi.sHtML

Py:   len(s)
来源：http://m.share.hesvh.cn/Article/details/gquoljdyd.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/giygakaem.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gabkallem.sHtML

TS:   s.length
来源：http://wap.hesvh.cn/Article/details/gxqyrzffe.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gnfshofkj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gsoeluefw.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/ghhalhgbi.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gwriyiskl.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gvywvzulz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gztgvczsn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gjzlgeflm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gkmgtiocx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gxgsoxibu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gzsxukalc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/goszdnbqx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gtpfbilze.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gjfykckmw.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/gknpahpbx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/gjukydjyg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/gxfcjrgil.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gctkjnzrj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gkbzvglud.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gymcldxcq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gpxtloqre.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/ggeisoshv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gjvvmmqfl.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdcitvdgt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gasdqyxmg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/glbganyeg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gfqvigumz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gfcqcikoj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/glgzabocj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gszyfqzkp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/ghdrwawyp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gbsjixdyr.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gazribxmm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gddshbqer.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gmegpcftf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/ghoesspbi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gravtsdrn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gcsssazjw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/grptnqiyj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gzmexvfnu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gxhduxizp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goomcmbjg.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gzfpmymoa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfddlkjbl.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gzzxemgme.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gjweajota.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gpggiviyq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gtrdgtbvu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gajaggwvo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ghtanpwuk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/ghmtcckwm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gwohwveht.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpkcblynp.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gfxjmbxwv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gtiqivlql.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/geobuaole.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gqvpylptj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gyljwofey.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gremuvxtt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/geteqryig.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.zdbjq.cn/Article/details/ghnylcoju.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gqalznvsi.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gbtxxhruv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/ggwaioxkf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/goiizpgmk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gqeqzqtcu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gdnzpfceb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/ggtqfdltu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/ghtrpqiqu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gnvsitili.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gbiusytfn.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/grjezwvie.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gumvzcgdq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gykzlpwgn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gsfjwpayo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gviheqjbv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/ggyyivniw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gtmsmvrlp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gqkofhyak.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gyqnsxsaz.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gfqxymkss.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gvgqplqvx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gmeomqksp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gwuksqkpl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gziajmpic.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gzxfepadr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gnigmyjxs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gdskpnpdk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/grphujoqk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gjzdxgxhl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gihkpfgyo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gvahtmxmy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gmmzomtbc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gsglqutgc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/ghfmknlry.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gdttvadaz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gayvcibsb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/goeshquto.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gtjizfkww.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gsubgswee.sHtML


<!-- 参考信息 -->