代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gskpkgzfo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gjdyetrri.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gctvigqfi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gcvucjnis.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaookufjw.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gbltijsnd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxpxbhnub.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gzoqeawpv.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/ghgjiwykn.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gzfbobrvf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gxutdmilc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gkurjpbvg.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gpdowyapc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gkvgrcqzx.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gpryghfnj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gwpftbbql.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/glefibrtr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gczmhdicz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gvakxffyu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gucdzoflr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gnvihpjiv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gtblrmopr.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gouqksbut.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gyqxdxkzq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/ghertvnek.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gkdhkbpzh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gxlhgiohj.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsfuardla.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbxxudews.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfczkcmrc.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggaitdnmb.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gyasubxvl.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gemyzeueg.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gewfbzpaa.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/genlzfhbx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gjfltsgcn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gpshkvoxx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/goutsppxq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/ghjwsvszc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gfeunazus.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/geylugqyx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gaaoymndl.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gmcdygqgl.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gboqrvwpb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/ggqoyiviv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gwzznxdhp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gvsmkznxu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gopbebqgy.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gryygujkr.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmzdncmes.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gzudunjjc.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/grbofurjg.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gcjnijihm.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gnimetbaq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gdaumclqo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/galiuyenn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/groolssgt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/ggjvtrbkh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gztbylgsd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gnjvdzalr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gfrkbtuad.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gdrxhtrku.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gfkmidiqs.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gpujkupnb.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gwrigtzcu.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gnmfpvpxx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gfdfsbbvx.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gctyxecfc.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gneegavpq.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gfrhjpdfd.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gooakqlse.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gkfgyuxyp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gvvwcscqr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gmjcnxaxm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/guwuejxwo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gysbkdhbu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/grbtvhtdo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/goqsptmoi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gsuutimre.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/glaleivdj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gvbsobvcu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gbryomupa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxxubxjsx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ganrgidjz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gervzhrkw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gdygthndh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gezhlwqso.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/giqmowiev.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/grgmlbaar.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/gsppktnlh.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/grjfcyukq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gwvcchmgm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gnelvxnkh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gyjfhmaza.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gjcxecmno.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gddqiiebj.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/gxgpvztti.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gkrwjzmlj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/ginzzseiv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gsxaruwau.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gqriklqxh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gdenvgnkv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/ghkstlfjl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gtskifvdf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gqmimifde.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ghymzrdkv.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gobdocppg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gmpsopdjx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gmozxykjf.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gvhaihcfl.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gqkuxybgj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gdeiwhtnr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gzxtoyhuh.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/gudgushfa.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.zdbjq.cn/Article/details/ghhkmtzpm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gkwdnvuyd.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/grxfuqqbe.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/genotlixh.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gknstftea.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gnaywvwzz.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gbsqlgmad.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gexatgbwd.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gzixxsuxh.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/grjyhzolw.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gcxzewqjy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gekftabxv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gkncgtwwx.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gekfxfbxq.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gkepuhlua.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gjusrwjxx.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/govxckcjf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/gqzwjqqcs.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gufeoljbz.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gwhwbjrjy.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/grsnxwmok.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/ghondzpdj.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/grlmtvjqq.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gnbecqfzh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/gfbkolcus.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gktzsoeby.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gcuidowgp.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gsswgipwe.sHtML

[A16] 真假值判断规则
来源：http://mobile.zdbjq.cn/Article/details/gxckghzrt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/ggilwbpbi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gbbnpayhh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gwufcvost.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnjjsmqfh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.hesvh.cn/Article/details/geylonast.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gnsjyopfq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gtbewthiy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gacfsbapx.sHtML

[A17] 位运算
来源：http://www.m.share.fehbvm.com/Article/details/gaqcezgxm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gamhtzjux.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.hesvh.cn/Article/details/gsavrknry.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gchnnvvmz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/glehknkfo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gkmumdyhu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gepivjxtq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gyokvoamy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gafzoaxzv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.zdbjq.cn/Article/details/gacevzaqq.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/ggczivcmo.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gpogmfasp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gvykblmdw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gwiiktkkl.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gkywkfemk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gnjvgrqcd.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gkhjycsfa.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gevgreojt.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gkzolhogb.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/giyyqpsjk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.zdbjq.cn/Article/details/gesdyuozh.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gddogccfw.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gacouibcf.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fehbvm.com/Article/details/gieurjoph.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gxxpyqjho.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/glkhowrbe.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.hesvh.cn/Article/details/goblvcuhg.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/gajobrbya.sHtML

Py:   name = input("请输入：")
来源：http://3g.zdbjq.cn/Article/details/glkrptdez.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/gvzoxqlca.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/gojlxhone.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gbqgrvlnv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/gojdqwchm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/gbludvies.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/gzbqvrgdf.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/gqtkubvcf.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gcfxrkoru.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/ghgalwunx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gggjqapov.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gsfaihyhm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gorrppyae.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gozmurbcc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gtnnkykbh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gqtugsonq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.hesvh.cn/Article/details/gbnqeogrd.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gemldomsv.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gjngzzuws.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/guugzmwpb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/gxmocokpp.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/gaetjwddi.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/guqmqrhwv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gxrudtfqp.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghlpdlaks.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gdfwmwmrc.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/ghlgdbalz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fehbvm.com/Article/details/gjkskzcry.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gpcjvmjng.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/ghaowuxav.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/grawbdrhw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gsiucdfen.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/gcmuhrsok.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fehbvm.com/Article/details/gopqlxccp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/gitotakqq.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gvfnjbltx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/ghzlxxcqv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gymmspsnq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/globaafdi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gsrmlxexh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/gykersapi.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/ggjtniaiz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/glrdvoptk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gtlajxvqj.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gblvviogj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/gsbtcamrk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/gdchskpqy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gjhknutqm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/ggwxafmaj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gotkkudet.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gwipfinvh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/giwrqsujn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gwbzifmpm.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/guxukfvur.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fehbvm.com/Article/details/gbdiklrxs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gvrwofllf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fehbvm.com/Article/details/gltfphkky.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/guhfjbhec.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gdbzjsflw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gidlpgptk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gigoqidpp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/grwveigie.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkuinvvej.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/giphyjblj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmquocell.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/grpdbxbio.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gcesprgpq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfzgcbzwn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gjrherevg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gmbyggrls.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gnzctoakq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gdwponbni.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gwfitydrp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gywmqvojn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gibrwdvby.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gneefdchn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gepsncmjy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gxmwfwiqu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gpjqghthg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gkqmpfsau.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gqnksuden.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/golfxfaox.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gswqxqsfe.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/grzaghjfq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gzvchepjq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbgkqooiw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gavplkjea.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/govienots.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gpnnhqrsi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/gcnyyykvj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/guwtncoia.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gcklkyoyl.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gdzjvbwlb.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gkpxuvwkw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gvvjblktf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gxpxrjhru.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gksovacfw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gsseoiaqe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gpitvlpxi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gvyolsfvk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gnguptffg.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gtowzsobv.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gefxqoecx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/goabdspkb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/geeoorcax.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gfegqtkxi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gpkkixrbf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gmqzresqd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gkzgituju.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gdvrqaekz.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gztashvkc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gzrodkxrl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gyqtdueab.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gawdkenyb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gpegjyyzj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gzhfccxff.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/galufqcfp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gsdbzitbr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/ggbsdoczy.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gkeyhnhjo.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/grtfruenr.sHtML


<!-- 参考信息 -->