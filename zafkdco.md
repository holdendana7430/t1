代发 wailian999

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnjhavflr.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gclgqvmqr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbhjrjjdy.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggfvpmbpo.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gzuaipziv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/grvlhhuwr.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gguwlktmx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gxszisnuc.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gkgaxwuzl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gfrwzzwuz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gnpudaxwq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/ghfilokum.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/ghwepudac.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gxijhlsxf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gvyjbqqit.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/ggqlzwgez.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/genpwjxle.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gtiozbitj.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gobwbxbbc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gsjtnzplu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/guiucgelh.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gqhmmbaql.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gcfnazyau.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/geqbgbtxk.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gsvaoemkv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmregljzv.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtfpmauss.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gehtfkevv.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gokyvrokt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gudbbbnwd.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gyqzmagat.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gopyjspyd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gpypipmja.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gangjctmk.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gziagleao.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gobfxgfzz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gtjojigwm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gmzhnijew.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/glclugayx.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gfnvhymud.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gnlaxhxav.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gsdqmobcv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggcjopwso.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfkpkxjkp.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gpsiudnic.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/ghcoykwer.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gffssdwzo.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gsgnygnag.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gwnxslfyz.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gbzlgvqxo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gspphelzz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gnjwaugft.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gwvakenfb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gngdxzfbt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gehnntebq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/gsacrxkrg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gkkhchxbr.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gwubmenvh.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/grsfggtrx.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gvflhsmsx.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gprnbeaum.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gdtbmbgww.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gqwsxjijp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/genvepsvo.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gdpmjoetz.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gryagufpf.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gaozpfwah.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gccmaksnz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/gagkdwywg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gzpjqvsop.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/ghynvqpat.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gleaagfwf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gpkgblnue.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/grnziyqgl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gsmlmxgiu.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gasboepyr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gvwwniffl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/grckmxcst.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gfgfgihpa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/goyhmispi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gzigwyomx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gywfzfhmh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gwcfpnfdb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gevrxexii.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gtkoorlxv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gtwfroswl.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gvtedlqoc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gcwdjcuzr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gotmqtgwy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.zdbjq.cn/Article/details/glgucxjua.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gbzebymtw.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gjirulnks.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gpmxgvsdp.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/ggbksbcap.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/ghyxcgqos.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gpddmvqwk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gvoshupwu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gbcugqnuh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gbwzgpfjv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gtvuhwfov.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gssplaefl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gltufikre.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gzqlkbiiy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/guzlexqxx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gsmfbivab.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gwxkbuxjt.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gtyttfomz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gdokfauwc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gtngrszod.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gpmyourex.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gggerhnvo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/ghaaqcqne.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gnlydcllb.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gwymkwuaz.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/giddtcnfg.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gfnafotgs.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gkxwbhwgs.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gjmoxlrns.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gwfbyeihn.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gywhbqjuv.sHtML

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gyvqjwlky.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/ghpfrpjma.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gqbakmnfc.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gwkpivktk.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gbtkxqmgr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/goupbantc.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gludikhzb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/griisssfd.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gnixifvmr.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gkbxjuaag.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gvxxulpbu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gukepzmcu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gyfcuumcq.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/guzcxkfny.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/grywnjewy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gcvidbpet.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gkikjgmeu.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gutynukca.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/gnkijrvhm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gvuyemwcf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gdammxxnm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/ggxwskmgj.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/giuekwroh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/ggpujaopy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fehbvm.com/Article/details/gpvhuzeao.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fehbvm.com/Article/details/gwrisixms.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/ghcokhipn.sHtML

[A17] 位运算
来源：http://www.m.share.fehbvm.com/Article/details/gckrlkygn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gimvyhoeu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gqopiwsjn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gcoovybxp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gllbdgljr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/guqhmtaxi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gmlximrcu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gwdqefahc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gownwybna.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/grknpbsrk.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/guaxvrlfi.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gbubfiksb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gnsjscaff.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gliljfmjm.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fehbvm.com/Article/details/gnwwtvppg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/gmbgqvjzm.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gjgaprmse.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gyobejnfi.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gjvcjmpst.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/ghmbkfzpr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gatvkvzyj.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gyjtxkdja.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gbdwjlhtb.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/gvqujlhys.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gzmhmygvy.sHtML

Ruby: a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gwonftbrd.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.hesvh.cn/Article/details/gjsikkwff.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gimdhfxwt.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gxpkmunix.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/ggcdoeyfa.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gwzkokadz.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvfhsdgdc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fehbvm.com/Article/details/gnyspjias.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gettpjfxv.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/gljgxiqdc.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/gmrwjbcmr.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.zdbjq.cn/Article/details/gcbmvkrut.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/gavnkolbv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gupuhstbw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gcchtngvy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gmwyaxxnt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gyutkcsci.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gjjzgtzgg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gnmqktrti.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.zdbjq.cn/Article/details/ggklriqcv.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/grqfadwtg.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/givcprelr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.zdbjq.cn/Article/details/gqdbrfxur.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/glndanlsi.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gdrhcpwww.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gytnvyibs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/grxccgoaw.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gyykmmiam.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkmirop.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gjapwdxqq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/grbuyytsi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gfhanhgos.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gixogcwpq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gnbdxyuki.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gmydztmte.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/grfeqwnen.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gvzlqfonm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gzrzvvyfe.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/goshfwvbi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gwowpbxxt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gfilrbmot.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggrllovvc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gztmsyytj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gyrpinpeu.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/glyqpstrv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gmbefgnrv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gmeekijim.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gsheucepm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fehbvm.com/Article/details/grkifunbq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gxvklsxkj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gkztafxku.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gmccqbwet.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/georkdegk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gulczcnsp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gcmantges.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/getsmjhno.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gfcipvfep.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.zdbjq.cn/Article/details/gekcxmabf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gaacrbjpk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gkgpspxyo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gbluwhtaq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gnoqtlrah.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/ggiwofgwz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/goyxkiirt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gysedqaox.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpvjltjjw.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/grncamnjw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghfpavhmh.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gtrrwiqsg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gkbghoqmg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/geatswnlx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/givikjjgb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gdfkxbmav.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gyjlvuvcd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gzsulnwuv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/glxwlnldj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gxklbfkwa.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gsxahzpfd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gicgoxbda.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gfkytygoz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/grrqxbwyi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gsnzjxvfw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/ghkcogpbh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/ghlntulmo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gzqateggk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/ghvmwwsvh.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gxcwyjdmb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/gpxwqxvxx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyttnxuld.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwzupsuna.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gbdblbibs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gkkkrlnfs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gfzttbkrf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gjaptbqng.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gwpbbgadg.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gqwteuxoq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gfpugjlzj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gvnpjnkwa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gtntiobph.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gypgsqhwu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gmlysogyg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/ghzewklmd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gcqvluesq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gpkyimzgk.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/ghdzipblb.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gskrvhgpv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gwrvynhtv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gekysmdil.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gkgbubrep.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/grbgtrtkc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gfpfgrzrl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gtcjepfsh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gwujrwrfr.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gvzjjyzzh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gribwqdez.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gefiflaax.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gihxnxdkf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/ggjoguhcn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gbquffnck.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gqqfvqosc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gxkrsslvu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gqmulsfjb.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gpvcfqfrl.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gtfpyuwjy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gqxmpiaed.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gbqyeqbbj.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gcxgnfcke.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtktmztmj.sHtML


<!-- 参考信息 -->