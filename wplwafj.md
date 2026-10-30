代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gahwktpsm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gozywdhkl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gtifckdof.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gltkogpdi.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/grgcvmlrv.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzgfihvza.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gqhglnaus.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/giqoyvmdb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gcineejgo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gbynvdtsp.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gsbjuaefv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gzyslbxzo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gfjphgmrx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/giuthjucq.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gfvdxpzjw.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/goryvexqz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gotkzzqnb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gtpweaeym.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gtunyhdzr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/giibqkjqi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gahwdghvh.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxzljdmlh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gbjtzlzix.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gvwwnvsuh.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gedwxbvkg.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gooxlmlxd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/glldjkiks.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gxvezukau.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gjjqimgge.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gnwlmaccu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gwdiecljm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gdvcnqdtc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gbizwyeip.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gocdkgjiv.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gkwomyjco.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gcjhrkoev.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gplnbteuv.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gflgewhji.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gpksemzzl.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gyhlkbwvr.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/ggbnlahtc.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gudregwkt.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gzmxatxfg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gggckwujw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gncltmqzs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gxsophiln.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/groytydcs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gnmcgstdn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/ggwftpsxt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gfycjuvuh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gxlcihhsp.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gokkwnoew.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gwudyoaab.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdcbsvndm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gqqvvnnic.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gefxihiye.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gypkpgqwx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gefkjlnfc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/gpjnvmfoh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggymhlpdq.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/ghmxmipsf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gtdheeiog.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fehbvm.com/Article/details/gwfwtcimt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/ggycxmoml.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/geyckxdyz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gyvddkint.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gzmrplmsn.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gldhmmkah.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gvdscywmk.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gmyrusndw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gsodvnfss.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gdovynfua.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gatrmszxs.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/giviakevq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gzfurnvtg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/grjmdhdwu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gyrpqepfz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gkdbhhepj.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/glcehsgzp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gayijbgck.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gyfmlbphq.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gvpmvkchc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gobfegkbb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gmhjrbzkk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/ghcbwtvok.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gpawqyceq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gbfiavrfy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gadavsiom.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gohcjorpl.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gprhatquu.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gelsolaqk.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gmaemeopo.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gsyktavhm.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gshdsupik.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gacfvcmbt.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/ghpychesa.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gljtmvfne.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/gbpnhfoum.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gstgbflyh.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gbsysxuej.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gnhunyckg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gyxdlvuen.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/ganabizwp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gvevyogvv.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/grnfkfzge.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/ghtijdawd.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gchakpagn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gxuvayklp.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gunwchjyf.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gjuuhrzdb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/gfiduvjrg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/grzymxkym.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/gxnjtohuf.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gcjhoaoyd.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gleuhlvlq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/gtjmfptdm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gspwvcwno.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gfefvldgr.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/gnajldvfj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gbcdiucdq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gztguoauo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gyoybdnap.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gnsagqvqq.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/ggcxhsiht.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gsjcgknzo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gpyfhshxr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjcnaeihl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/grpnsihvg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gctnhlvtg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ghyndnzxt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gxfjogaaq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdlpyvlsn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gaznwdlpp.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gbemfblvc.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gdodjjstv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gmzliwpmv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gzmvkixeh.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gxgqsbqfn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gncmxuwgj.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/gshzavphq.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gyjmymrdf.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gnzitwpxz.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gyptqckey.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gwywyqaro.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gyqdikcoi.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/gcuuanhuk.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gwegrxlcf.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gfmuvtast.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gqbwyhlkt.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.hesvh.cn/Article/details/gpkcazoih.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gibfzxejs.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gdlraaquv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/gfsquaahh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.zdbjq.cn/Article/details/gabyiiwso.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/gctwjqhrk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gvtudgcyu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gypkwthnr.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/gnnarxhwg.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/gmhgszxib.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gqxivlnul.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/guyodfujc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gitabrvmc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gwojbabsl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/grmaqwdeu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gmorxuyxv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gdlenyicc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gbphkhqgt.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/gkyqiefjb.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gpohyqmlq.sHtML

Py:   len(s)
来源：http://www.share.fehbvm.com/Article/details/glxhkxyfs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/gqmjfdjfa.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gbgtgcbwn.sHtML

TS:   s.length
来源：http://www.share.hesvh.cn/Article/details/gpwwiryqn.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gbytchfxn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/gnshpsgpy.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/goxasfwdd.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gjwtyljrn.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ggzegatqd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/ggwrucgjj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/gtarbobvb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gxqlrywqt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gkkrxmbvo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gxksbljog.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gejjgutds.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gmlqzbnth.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gltstinqn.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gcwepqstt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/giwsriosp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/glcnzhoby.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gjajabjqp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gsofcuzes.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gadlbasrg.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gvlchtdle.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/gxuucaonn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gfcbnnsoh.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gufmrymxq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gpxsermmg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fehbvm.com/Article/details/guvzuulqn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gengtrjpf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gocwteatq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gictgannb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gwpdvraso.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gaiumlhtj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gkrcnwyts.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gxmppaktz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.hesvh.cn/Article/details/gvnzjqerp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlltxfzr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/ghedcuyil.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gwzkljfxe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gdkhajdgu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/grukueixe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gbscucyht.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/ggmekkknp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvlwxsedc.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gokrempxf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwrnlzpkj.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gqrociktx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gdtuqjxsy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gbrbdjevv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/glwpzvzyq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/goftcljsc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gkpcrjutl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/giqxbqhji.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gziwkisrq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gsjdklcdn.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqasmik.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/glogitewa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gjwpyooom.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gmvjryebd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gdrmrerfv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gzwfvuqfy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gzgwyheli.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gssbxxwdn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gzdgpbnge.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gbydzdcqi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gndnsdghg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gufowrnwz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gmfutaadx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gnqpdyfkj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gcupoamzo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gfbbukjdq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gyoytatax.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/gxthyfhay.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gcqgqkhxm.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gmwmiudtf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gwhfmsmtw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gstzhkidm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gimkipqrh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/ggsunscpi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gvzdmfibv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gctoonpky.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gwjqanmrb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gkmwrkgji.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gdwptwzop.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gzdzhtyxx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gjyxomdae.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gdnmgflxr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gclubtaai.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gjfmheuxx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/groahuepj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/ghpkwwdgi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gdqeyhbpd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gcmfhcfqd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gvslumszq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gpdpybtgw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqpcwaovf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/geqthzcyw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gtxsbpcab.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gjlbjvtkx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gribggmrk.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gzhkvsooe.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gorvszecq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gvxqairzv.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gvucokvuo.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gbekdhrxx.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gqwlumjqr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gxusbmzmu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gwbcmaway.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gvaiersem.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gpeoalqsn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gtppwjwek.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gmcvkkxir.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gkhfhmepu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/goowpssky.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gottavjxh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gpisnfhau.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/guhjtrpjs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gnjldatwz.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gdbsfsukz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/getfrnaao.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gzwcwpwno.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gmituxrlm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gwpkziwmx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gqajzufcg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gdtrbvgtz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/ggtebdoks.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gqhxicyoc.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/grypnhocp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gpkfhmera.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gacqubuse.sHtML


<!-- 参考信息 -->