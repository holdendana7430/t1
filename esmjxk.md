代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2bloxzbke.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2soynxzbx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vkiwiewn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rseqrraq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yajrnhxu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xfwtzjua.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ooymyuna.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ribnknxp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hmgwhgxy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hovndhyv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qwcqbufu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gntkawpg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oyhhejlu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ljuwrfqv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2quznqqec.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gvqussrf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wqwnpxio.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rnudurwq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pidlbcfg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2abxzdwon.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2iwkrrwqr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xqkenmnj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zzvpynkq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2zlpephkk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2yfoqhsux.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2yutdvlxq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2njgmplfr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2eqodnoif.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2yrnhofgq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bopezgjv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bxukwlkj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkhobzyz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yqooeerd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rernrpap.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lkodlkkg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lailexyt.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hzrhyuyr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2udadwuvo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2fmhdrtrj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2scuitzbv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2tvxhilzf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fmojzjgk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fvlfxvco.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2lwfwijvt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lyylfrpu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2acjmwgxs.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2munooxvf.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2itmwgmsh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2efnmlxah.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2mztbdwuw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qivhkjge.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdbdxjg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dehaxwqm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2huzukwop.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lkarajfz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qjmhtrpv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahpwnzqq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mujikxdp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2tzekfjhf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2asvmetjm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ixwsletd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2akmwlgah.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kxcrfkbk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lsejazvj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgfvmpk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2efkibwes.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmyymbnr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dapgqhsa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vlradeue.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2qmkhhzln.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kdfuzlwj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjlclmyu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dkleiwor.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ygwxuhtn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2fsscxefb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gmeuspcw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xsetompx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pzujdrdm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2twnyixhi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zzijepyi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2sdrniejt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2cosyldbo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cvrwcqnm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lwdqmtex.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cxitiqcj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iiefmjeo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2guctqgyt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2cnxxpfag.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zywmyzrk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nbvielig.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2omnegoiy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2cjygerul.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nuebipoe.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bwzryhsi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2epagjebt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jknwpcmj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fngwqqmt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2pkchwumi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rnzghkvm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xfkxbnbn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lmttzfby.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lpchymlf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vzvyxhgw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cnogeysi.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xmpiwyxt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jlhkkwfk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hbvmvzjh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zgmhiqqt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2oftxtyvs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2oceohjoz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bphgnitu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gdzlyxbc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rykzwgfp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2uxqftggh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ycwzdabr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ueoxtqwg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qxulyice.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iwwxssai.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uvfyrido.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vhhxwfgj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vbxvytaq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rjywfsuf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qywvnhfx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2iorakgom.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eounjgnr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hguttrzi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2sklydysa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2trbdnicm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2gnfxgejt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2incfqkhy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2mvinsnyx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdxeucsg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2onbjtlad.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ibkxrxsz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ausiwztm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yzvsoaqr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ltkeqsoi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lalopqdt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2miftrwra.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ixykmfpd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2apwfhbdt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bcwiucmh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rxhamsyv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2beqjtncu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2yvvyggfy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wbxfosaq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nohtkifp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcrcbjd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ichlzreo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vqixhmee.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ypupwnlt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2jgijplcz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jeakpitp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zfhanabn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ongfyety.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mnyldgdr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zddrecce.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vzcncrbe.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2muqgpybd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2easruiku.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wxtckfcu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ibbqeufz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lmwizmce.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2qqezjydq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bersqmnc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ejodembq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fganruyd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2sfrzqtfy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2mvytsmnl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2skzxhgri.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qljleens.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jpssegcy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2aqqlsbyj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ipawrwlu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vgemtulc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mndmkcsb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2adnfisiu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wkfaprex.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ldsaqaau.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2sksbdxui.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2snqsrgvw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbccumnn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ktbobuzc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2diwvihfh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rcwmatem.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fmvdkdrg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahdaksow.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nnwhdkwr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2adhrucna.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qwznyqbi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fjihsmvk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ffyvwxed.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2emrzzcxy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2enjtykjk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xlqwivrn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uwwijspy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pdgfcdky.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rluyrmor.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ozeinzse.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2slhxfojf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2dncylyhd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2izfjurle.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dxmnkrhb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tlbyzzkc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kvxxztkc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cpklspqu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2brqiftgh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bylagmly.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2vxabojtu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2micnqhuh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rqghlsat.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ivbypfig.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhriwyb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rbthwfbm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2zxjilmxp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gwmuqxpv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qbxqvtla.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ocmnjftv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2sqmsihbp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2faomqpju.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gjulaoxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2egiwyfjw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2sjnvcsch.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xejkyaak.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2edzsthvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpzdxtri.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qogftcqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avzykmbk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jwayisdn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tqfxispw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvclvodh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qgpaeizz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ahdkarqb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fooqfbjd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpbpipzg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fecqmyuz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gvtgguay.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hsqumugc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mcqcdqcr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2leglvxqa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rcjxkxyo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rzyqfesx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qhfynyfo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wkvchbtb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nfpcobpz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2twoliprc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ujhuzfgv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fnjrwfji.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erjfulhv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbzrbsqu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zhqwczpu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogkokczf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uyxmxalv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qmoqpgeg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dmiplcsi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hbnssewc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wrxbhiek.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2csuquoww.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yhggsksj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ubnpurqc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxztymws.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gauhgkfw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2itecnyjg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wbhilgvi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rvncchcj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uocawkwq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tnjcsloj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaqttoza.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jgioqfzr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hytdbyhp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rlrifojv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2apbrhkwn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpjotcgq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2oanqicbo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tqgpfmlt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pbmcrsjg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ulympvws.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zldzimsx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vvuimdpj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2eajjuqqy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iucqserb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dxmfryqt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hxpdylkq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgxgcykh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tpbouauu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykktkxhk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqzrbtud.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jcitxhdf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jgvqfqbf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wnxwesen.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uivapmje.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2lfvkkgad.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gbdxexpf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2llcxekin.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2obhrkkic.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sisbegen.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lalgzizg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qwtlwpax.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2pzahtdec.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xoevyjcr.html


<!-- 参考信息 -->