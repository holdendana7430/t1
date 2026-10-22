代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ynttacvb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jrblhnyv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2uuymjyec.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2iwrkjhib.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pemqqktp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lqcrlyzv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vcirnejg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sdnlhtgo.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bpsoivid.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ldqrxihy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2auchpgwy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lptumjwx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hefsxdpq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2utklhpxj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zroorxpb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2itdbetiy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2enbzwkxx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gsnldbyw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jxkfmued.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ffopkjpk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2cfcvaenw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2oswsablm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2splzgulq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2mqmdjelz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ffwhhotu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2reaosbwg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zavldhcl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rpwxmljy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2abednqiz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lgkmxkfm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rdpgeqkx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hpqusywj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ouonamee.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2emsbfapj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rudkwvfj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nudlhuuv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jorglogf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2aawtryni.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cvyiovyh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vwmqrexi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nrqwjmxu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2asfivrtg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tgnslziz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wxcufmsd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fpryyvpd.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qhkhvwiz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ecasithx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vmpwmfam.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vxdyxrii.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xvyzpsex.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2eivuqhql.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mhwnqptn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2nvmrujms.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2amnikwie.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mmmnovey.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2spkjvugh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eraqzogs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jpvmwgin.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hpqsogfb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2atqtpsrr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhamdcjp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdramenv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lecfwnsj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nepzkvqr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2onutzgdx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2gojtjibo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cqtglccb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iuasrjov.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2grirzkxo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qtbcywrt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ajqbhijk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvvuywgu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2izhbnnwa.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yrhuqbnh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fqrscbnu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ieqsbyit.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2oukcjlss.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2aaaaxtdx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nvmylitm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cppshsjf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vdnxszzs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zklxbrxc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2twtobarc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2gwnadiin.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gcmrtzwd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2joyfozuj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2txvazril.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2fvlnpkhz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2apcurpie.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2udjiapww.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2adnawwkl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdpsfhl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2lzdmnebm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2uraxwtjh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2octokngv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2klebejjc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bxodagln.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2upbyoaxm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2olcwdtrh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2htsqmshq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lehgpaqo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oihlztuk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dxzvrsfk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2axddmlpl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2yamjdoco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2sbzqewtt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gqftypfw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tdjplukq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dtuqzgzx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zfrcdehg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cealrkos.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vxuonmbr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2emgoduva.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2brmyxpiw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bwffbrqn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vrnyidwa.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ahvzdjjp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tmwzslwg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2nbvwsbyk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zhmzoqde.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lsxqdlum.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oemyfkae.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kgfpbuiy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hokgmeaw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jqcnlyuz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2khelwzeg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2zwgoxgev.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwiyywfc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2aqmnxyxu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mludclrj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nipalbtc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tdgaotal.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gshnntvi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qlubeizn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2situbgqq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rzhakvvc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qljaosya.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpclzrrf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vxvseasn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfjrscrh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2msytbgmv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zarqgucb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dpzpisat.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hpgsamls.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pvflgfls.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gejsgfyz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2gyqdqpmm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2jzaqzfgq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cexfovvq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2hiuxxqcm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lyociiqy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2lthlpqxr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ngsgaieh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2iqpgmkgj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2estrdkye.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wrpeqssk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bnrhqzor.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pgsyajii.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2jwmgxniq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dkephlce.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nctcvhly.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2nkmyzkvw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zvavaept.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2lrqsvnno.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2eetgqowz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2snoyiigw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2cjnvcuyr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pqmobbuh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tgjlgyex.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hijgvmqs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgbczyb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vblanzfi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fubduwjz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nsnufkhg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2smaysjku.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hswvagtw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gbxrnsiq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvnnszgi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2yesfqeyi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rhzdobgh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2cbcvwubu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2prplemky.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xqoaemii.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wmksothz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2trvgaqcf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mptfcwry.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jgnlzxic.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgztnlli.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nmelwkvq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2axceabim.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qbevipkt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fpewasjo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2aeagduwv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ctzljrqd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dqbhisbd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2vsbfenii.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2erqzvqvg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2swbpiegy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2famzxfav.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2anjyqfrf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2gbwaakgt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kkrmambh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zjgvlpeb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uryoqrup.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hsptktvu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghbkhirg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tgntsxar.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bsspapbq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mzpfqutf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2senlwneb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yjfubrsh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgaqmya.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2pyczwayy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bdjqjboe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fbzpljos.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lhxrcnzd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qkllgwzo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvofzij.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ommnxxbu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pwpvnehc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jbdzsqbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwrnullz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rrbnvqbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyybshst.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jhdeiywi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2zykboalw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxfejpio.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wvpsxgfv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kskxjxfm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ppsgbzgj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gmskgoko.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2frdhvszm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xzzwlbwq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ogzaznes.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2phqzxyoo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gibcfrrt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qqyskobw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vtysnquf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bydqnmyy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrgvmtte.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fsjngqcq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jlvzvxcc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vqviedmb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2iiguwbqp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ssmhvete.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjkhozla.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yizwfije.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hcdhbieu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xcpolmio.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2vlpnqzkc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vubvnqym.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2isjjwxrk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ohfarbrv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2esusizje.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uxkxqkcb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbkedrtr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2foxdehqz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2owixoxsm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2nwasjgdm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2otfhrgpz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2saxipasq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrysikd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbnmebiv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvjrqbhv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wexkhsti.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnwqlvnn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ezardwmb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lvtfccdo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bttienrk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zosctvqu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xtuqyjku.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lsuurqsn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pqvqqwcx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruacstxf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qgxcyjqi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfpdvkiy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lyglmjdh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikwrqbyt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bodvbdhn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkluoipb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2feuwgibe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2whekbwyu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2itujjimp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sigobtgp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lltnqqxe.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndjevhvy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dxymryhb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bsdikrvx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rhwrpzxm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zbkijxgs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eyxzftnv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2slqonbve.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qbtzrjes.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2apqvamvy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2derkhgvu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mffmwldp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bgdtxhpl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zqkouqwb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuzixfch.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wwimhjbn.html


<!-- 参考信息 -->