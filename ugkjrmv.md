代发 wailian999

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxdiqtbeg.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gystzlnrs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkbiqbgoe.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghyucabgx.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gzmstlfan.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gadafszqk.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gnheevflq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/ghzzapyjg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/giotxdmyg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gkzcuwems.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvcfznt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/grstvvyet.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gnmvxbzsa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gbuhbyhkx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjagworrf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gydxflvsf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/geuohvwrf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gjucaseno.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/geathtkyo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gvtyjsxic.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gayyjibxm.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gqalrgdtk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gmyxbjcse.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gvibtscqy.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gdraaeivr.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtzmfnqbd.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtpgznkuj.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gsitwxopk.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/ggzqkpjer.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxqkgycmb.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gpfnrkprr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gwdultqrv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gxbvqloxb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gnsauhfpu.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/glbqcdzjc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gjlootyys.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gfodbmrws.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gfiggbcnk.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gyrnrjmar.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gtflujfde.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gfudntvus.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gnkioreyf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gvzlnaabk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqqahezjp.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gbyvguyio.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcdqscscf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grqdyzvod.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcxkykuqd.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gdrwkaxto.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gvgeyyhtu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gvstpmgmg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gdtywgndm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gvqfkajyg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gttpiicbo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/girfrgwdh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gnahhslyo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gdsrouatq.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gopthtyhq.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gnzhlsnzp.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/glpecrmbe.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gootrwyey.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gxazlviox.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gnxiktind.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/gqdgjxlpa.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gyyfqyiyu.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/ghpkfyogf.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gpbzqtxzb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gosfoiusb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gaovoggkz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/ghauivpze.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gsgtxairg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/ggnfuvzeu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/grrovxbmm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gckwnieyh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/glppukysf.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/ggxelntpy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gopxpslpd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gzexsdhgr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/goiktfwmn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gsbzpthfg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gbytheaks.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gjakjbmyv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gyiinzqmj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ghyjfwbwp.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gnapkgrlq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gpurxizwz.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gtzntezfd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gytstzfmg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gudfusbde.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gtwcuxhqq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gqqdxsqvj.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gqkxbyehf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gpcvqjzku.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gjgpgefvc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gcaagxytv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/giqsuiscy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gsyaouwjv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ghulxkevg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gxbjxebyl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gzmumhwoo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gsuxyrftk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gahajiejd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggrwjomjb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fehbvm.com/Article/details/gexkeyrpf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/ghsgvjrsv.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gacmzqtyi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gvnfrfybs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gazduecgi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gyycbtlbl.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gatpsfsgm.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gyobldrrr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gfzdzlenm.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gqztcvbjw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gicafyfhe.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gtlwuawan.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gzuegwdff.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gxpbawkqp.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gsrydovbn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gwrgemwqs.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gfavpefmb.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gfwjmtquo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gdkjhdpns.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gvsfkhofm.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gmxjdiuaa.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gqcarqdkr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/goyixylzo.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gvbbxzfpy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gawkaxhzo.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gkbpecisa.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/ggueqwyjl.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gobkbojhy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/grdyqkuzt.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gtaxudbkq.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gpqvkncwg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gjvjqesvi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gmlzilcbs.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/ggeammpcb.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gnapmpybm.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gnfayvnqf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/glikhfslx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.zdbjq.cn/Article/details/gecbhmztc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gpcmtejny.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gnskxycws.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gakjhvkpc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.hesvh.cn/Article/details/gmlrgmkav.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gbgwulwkc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/giymvvxqn.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/gisoaikjw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gapaxnxwy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gekkzxmjg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkstvpkpb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gfkhxyjkx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/grupmlotk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkxxyakng.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gkcdzomdw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gtiiknmqw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/gcvrzftwz.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gciqbhrcq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gvtcwracx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gsfuepqvh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gpvaaxzej.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/gygwmyged.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gipqigaad.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/gpvfjsgae.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/gxrczohpw.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/gimfywdvn.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gkkdzyssk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.hesvh.cn/Article/details/gfkjompaz.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/gujsfyike.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gitgntlrh.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gpeaelwka.sHtML

Go:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gchtvlsoh.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gilvbuetu.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gzfgxpdsx.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/gahokninp.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gwwfqlwrs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/gckjungmq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gebxqwfwp.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/gittsqjhl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gfydxgmwv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/glapuuwnr.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gwipcjlwf.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gvxazadcj.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/guzontucj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/glrhfhjfe.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gdtpfsouf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/glrylxaud.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gbjwozzcf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gwuneowsi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gxosjuftp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gyelrekso.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/gzsvfvkjb.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gmyzxlfvj.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gvvdvbzct.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gzlbecqxr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/gqwslozdy.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gdmijonob.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/givvdcjnn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gepqznvvz.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/glsvxalsw.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gvatnlxvf.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gdpkbdyro.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gffoxrmhg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gmguitpob.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gqeowxlof.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gndyusizw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gyurqrpoq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gynqetwjc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.hesvh.cn/Article/details/ginlraqhq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gkatscwmb.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gfzmutina.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/ghruhsylq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/ggrfbuert.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/ggojocwim.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gfbselhcd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/gzxyvqstk.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gzmpxekoa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/gsrkzhzrh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gjhufrxfh.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gxqslmcyg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gcawjewcx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.hesvh.cn/Article/details/gijywnnbh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gsjnsired.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/grzzkypzf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/gvbwkomhb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/guavgiqsd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/guylxjory.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gfqgdfbtx.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gaztaekei.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gcbdgpgxw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gysmcarui.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gmsnkpgmq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gsvcnxcbh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/giueitkdw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fehbvm.com/Article/details/gjfzxlzux.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/grchtkhtl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gwhcdcgwi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggxdlwrgy.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gxqizumgm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goomibuof.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gtzeniamk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/grwlpspao.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gbnlniaju.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/ggteadgvx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gwpklygao.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gdorvkmji.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gjbwizxny.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/grjldpxjr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gmulnfuoz.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gktrkpueh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/grubwzemn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gqruywoil.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gaollvrnc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/ggcilbmat.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gmezchlwy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gnnxiumaj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gugbuwmyf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gudphiefs.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gwkguirkr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gqtefdohh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/glrnmrpbm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ggekysclp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gyftylhff.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/giypputhv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gmaiawxmm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/ghpvarblj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gvtzpffqx.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gbgylifem.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gukvhoryk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gtnaszimp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/glnpfxwpe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gqoenpxqo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gkszneokp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/gmztveqsx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gvxfdjcsi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gdtyyimrr.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gbrgwcbxt.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gwijjexen.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gvrmqryjo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gtsebeedq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gfenakhoj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gzepqanwh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gtgobkfls.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/ggxfqyytu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gzhpyerwh.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gawvbafsj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfdjskm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gwyvmwrdl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/grjjfuamf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gtofagzqo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gxseqzlpc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/grfbiqbsk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gstuqumqc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gimajvrjp.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gndaustub.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxlfppxaj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gipfzokph.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/ghbpaunvg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gzcsgtzcm.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gkrqqatci.sHtML


<!-- 参考信息 -->