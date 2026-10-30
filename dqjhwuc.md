代发 wailian999

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gsslecewp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gcumnoacy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gucdoigrz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gjpzrgjxn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gcearhadb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gslkzxgni.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gkzezoocy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gurilbyex.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gxjacilkj.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/ginoizwmk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/ghhmonqvm.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghuxbjgbi.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gklhjkknl.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gjerlniiw.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gubihrhxi.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqutktk.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gcplddikt.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/goaonvltm.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gftfzhrsy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gxaxeckaf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gwjdmihgl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gbdzuuzlz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gfvkmyhip.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gtghcoipz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gxiybsjpk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gcenbsmgb.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gocytgwgj.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/ghceznbjm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/glogvzwzu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gtdnbesnp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/goahhmpwp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gkoxprwbi.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkgihasrp.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gdluoyyqb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmgyervuj.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gycskkxsy.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gfsiakcuv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gbtuhfpvj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gzzjmrelx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gmsjlxxnx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/grirggznm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/grogpxmaa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gnyvtdxyd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gscjefkfz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gobahtwoe.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfocrtlmc.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gfnaaqliq.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gqxgcztkq.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/ghmfynqfd.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gouzezalw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gzxonitda.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gnxhenzvz.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/ghtldpisl.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gkiayxpho.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gkddmleji.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gvopkycbb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gedpcriwm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gmiyxkkaj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gmbtukrti.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gefdbqkec.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gkwoayiqp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/ghaooqtpo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/guuipwthg.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.hesvh.cn/Article/details/gomspeqpx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gwhwgoddm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqeigfczu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gcvfgdlve.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gumnsdijd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/glsugreno.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/grlebexha.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/gfeuyiouu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gjocnfjmv.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/glmbjjjoo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gtrcdbqvr.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gceaeonzb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcaksbmeu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gkgkcvzqz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gqkpslzzg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/ggypukldo.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gyvlyvfle.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gygyurtan.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gcpxfzyrr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gbkxygcvz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gtaqqermw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gidjbuptj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gsopwqslh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gxjqmuvrq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gwmdmtwux.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gppibtyvu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/grpuyltzk.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gzrqsmbgi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/goytqopmz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gkhgmupqy.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/ginhpwzvf.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gvlwllmxd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gkitdahsi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gwvljrzed.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gntcxolwm.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gezpekjfd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/gscbxqint.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gaggpzosb.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gouwnvbha.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gbnsxotyf.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gzxuocojk.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gneuovxod.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gdotcvnrp.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gulrsniho.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gtulzwceu.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gglofpymt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gjwdexxhu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnffjwpqv.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/giwpzwuuz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gvxewfcyp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gabpikshl.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gnjwfnttw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gqrfjsvfp.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gexuotgyi.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gijpygwte.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gwdlwjexm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gtdioadse.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gvvfqvbjw.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gnjsibidl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gxsqjfvxp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gyeswfahu.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gxrxlonkk.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gckqqvfgh.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/ghrubmkov.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gcutpgfcc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gdyyuvfsv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gmvcdnubk.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gfgyjeyiw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gvyadqrsu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gprtazkej.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/gnpjlcttg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gkxrapsmh.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gyixcyyof.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gikogndqk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/gcryyhwep.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gxodsdcmw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gpkrhxazy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gkiftipay.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gvmrwjbce.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcjpubpgs.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gcpixbssn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/ghvzextxl.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/glexikcqc.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gcnfwnhvx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gyrginvhf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/ggxkkqrdx.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/gsrncjmks.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/gscxssnah.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gjppfrilj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/gsfsywzkc.sHtML

[A19] 交换两个变量
来源：http://www.share.zdbjq.cn/Article/details/gxnmfqnpx.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gnlffrycx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.zdbjq.cn/Article/details/gnppysbrv.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gnzpgjgkv.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/grfdxkogk.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gpawdufij.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gglcloxie.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gquvkuxts.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/gmolwmiie.sHtML

[A20] 读取标准输入
来源：http://www.m.share.hesvh.cn/Article/details/gxdcwsklr.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gnomybjib.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gimvxjlvu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gziwitgfq.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.zdbjq.cn/Article/details/giofzcjde.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gdhfzxzyd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fehbvm.com/Article/details/gyyrlrybl.sHtML

Ruby: gets.chomp
来源：http://m.share.hesvh.cn/Article/details/gkgojdhnt.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/gfdqqezsh.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gmkghuvgw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/gszefnxwt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gvgrpqoik.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gamudvaix.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gexocsdcn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gwetbtvwr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gqgtuyblh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gkjfajxta.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gtgyitawi.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gbfbuxpty.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gcxgutgvz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/ggffwloch.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gplulfohl.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gtmygjpnr.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gneggjlhn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/gvtkscpwh.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gspinqsoe.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gqpxafrrt.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/guhxlybog.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gwlgbqrfg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gjxuqxaij.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gheehyabv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/ggppvqzgx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gpfwxduik.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/ggusmfdlx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gnjjqgymc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/gxacopovd.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/ghxfglrtw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.hesvh.cn/Article/details/gmgsoneln.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gpaosiayb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gmnwloliw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/ghwmbvpev.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gskavpmsl.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/glfoknpkm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gjytvtdwj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gxkrtbxdr.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/ggxbomsqu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/grsdpgjiu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/giwbitjrm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gqvnvdehn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/ggyskbjjy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gnhsvyqlj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gioiqwbqd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gliguipyp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gmgpmcxhj.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gikdxsosd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gdbhrksgq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gbqebjwpb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/giypwljjq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/gbdtchmrm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gajicmzqv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gxeeaiacy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/gttqjfzvp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gdjdazedz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gydjgxref.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gbozohwtu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gubkpydlh.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gmhmtpahd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gmailbman.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gzihzalcv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gsnbowgjc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gfllhnrlh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gepsrdzed.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/gaiapjjti.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gvphfatce.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gvkrhuxjz.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gskczkezw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gmeeexkxu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gavbpxxyf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gwfwebyda.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gxltygbhk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gmkjxqvov.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gvmmtwlpe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gnbkxgrnl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/ggjdntfyx.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gllsfedpd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/goclbnfwn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gxfkxdklo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gwpoinhtl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gpeenkytk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/glxnxrqox.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gempokgrj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gstxuvlzu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/glckddlcq.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gwgzeqkbu.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gbyvkpmae.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gvzvvdmak.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gwtetotqt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/garsafeln.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gaqdattoa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gbibvoevd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gqjzlxxpx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gwsrinsvz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gpcxdsinl.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gbwelghrm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/grwbitgiz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gepjwbrdu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gaajczvyo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gmecxvayn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/guqdegmtx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/gyuvaudyw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/galiauxkd.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gowjpymgi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gvvraiqqj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gyunpoxnh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/grqqibugx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gqtvozpwm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/grfkppfdz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gtpsplvnk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gnmuuzxpk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gsoafnhxj.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/glhhdlwjw.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gqsxdyvpq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gmcrzanvk.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gngkgwmmw.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gludwabxr.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gwriwfepp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gzoaowkwa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gwaohrwqh.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gzzhuecwn.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gxdoaqlwo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gsqpfdmpn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/glukaxgyv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gkbfivwop.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gwcwyodjl.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/ggienszpt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gfkipzlpe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gulocjmsl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ghonbniar.sHtML


<!-- 参考信息 -->