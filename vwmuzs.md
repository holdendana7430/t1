代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3veczdppv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3gmpwzxzn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vygojkpd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ufunfgwd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xzrzjyai.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3shmfjpgo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jylzguvb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3trrvskrh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3itgfcdwl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cenagjgn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ncanzxqo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zxdsgioe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mjsetmfn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dfqezxyq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3foikcbnu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3gepgbodr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3stmwdrwu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wudogakv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hskwywpv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3azcqmkyi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3yjcjluao.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xcbafduu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mwaclzuo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hkrtxfjd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rysbqwyl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rafglmhh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xolgiffh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hzhlohli.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eaauiddo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wzliibsj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3gkodcbbg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3npepeyix.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kxwnssoj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3chyqopiu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hznliqiw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3dygfobwe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3voipfpws.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rsewxqti.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3doyupawv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bvorynmn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oayxcmne.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tvmcyvfw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vdrunbly.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3sgsgfxyz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3inrdnznj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3lcatjtmd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3pqreabyj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rglvdidk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfgqnxmb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkpwkny.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3thcfomel.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwngxps.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bpdvhxxh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wvmaisbi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vtblnaju.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hviohthq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlgjzkp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbajuihv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nopscroz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3upyeqszc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgaiznwj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3mukfceur.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3fvkuzeln.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xngupssh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3aijqmmif.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3hixdchfy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3xzulpjex.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vrlpfbrr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3igsnvjcy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wognnspe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3iwlxijcg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmlbhdr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jmexxdkq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3jcoawayq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wnyiitop.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cuzufyby.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zvkborju.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ciagxbda.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3darjqvej.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vbhqofdz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jnbjblne.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bbspvkuf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3sfrvhfhj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3quevvopb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3auyhwjur.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kxzysvll.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gjsiuvgj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xvwbcyav.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wxxpmeup.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3isokfycg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3upbwucye.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3zbuemkiy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gtsfhvto.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fzwohkip.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vlxptlzc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ybiffgfg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lvuqvzsl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lctxrooh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dbojqpnc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mytowhqk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tghqihnp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ygjcotbz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cjxgiame.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3adpnvnwh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3owvxmleq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3hprmzkxp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cwgzxdab.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lyabyntt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xobhjzai.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dricsgpc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cnmgxpwx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3olsyxuzn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ougfismc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qatvsgwz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3nuntirns.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovgqyqbx.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3umqvdrqz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yvqtjmhd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3adhqfxgo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ggxufuge.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pxtpyovn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3guwyvrmo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vaqfdmac.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mcysxnzi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3oniaziyw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zqhhgcco.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywbslksq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3zrpcsymo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hbmzmegk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3csapsbra.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kuhtntnz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzgvyhlr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxzfqzno.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qjzqgnza.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3plshayby.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ajmuowtj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lcywfljg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mtqzuhlt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yjdbytms.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ekxdpcfn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ecruwvqb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ptfkzdmh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3mrktdnbd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kbfkugif.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3kinuszer.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jlpwllic.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dwosvmhc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ludegvpf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ngcbqgov.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ixyjtnkb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3npwsoasb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rdioufwr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jcgwdzdx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3bktauqdi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3keavntjp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xexbnriq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lwgczmme.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ytxnbysw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jusqosfc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3qsxxxgcs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3amfoorny.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vpeuuqwz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xffsvjre.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3umpmdrwm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jicmqoyr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dajxkjya.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdnbmlja.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3guunbveh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rxfuntqm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjlqxfr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gvtljckv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ggkuqmeg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bqqdhyno.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3dxfflwgb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3irheamfy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mtcdmavo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ncamwxfs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3dkfuucul.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ocghmzhg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kzacdcyr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3lvzoyfkc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xldcjqdv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zqxmhcuq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3agbfqtkg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3peqwvvjf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jsrfeclo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hfeohota.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxupwyno.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bxhonbsg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3mmxkhczr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3klzozkkk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rhputwyk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkonngan.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kcaezdol.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nlzkvhmm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xgthtdqq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qnylfmho.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3yizajdfi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3awwefojy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3udmmlgki.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mwbgzhwg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgxbffng.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hmjrhqgv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxhtezl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqzzsgor.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oubrugzb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fqgadhyp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhaptebs.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qdhtwzvx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tmtxadpx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3knxgsawv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vnfcnbqg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qehbbecs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nhxwzpjy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tuhhuiqy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bmqhnojw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ofayimsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqlqjlcv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ctthfedd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrhivuay.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3dtnadzka.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vvemtabv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfleuosh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uoykjnsx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xrjdligu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wjhqdifk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbueuvvx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wrcsoaec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lrgotqoc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3wcoyakqj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qcljltgt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psjcxctm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mkrizfjh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3daaxijro.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vvjylzyk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3juglgqcq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hcorvhoh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ihhphjcp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3einbqkwr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hxtuxlfj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlxuwyfx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqljfmpw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sllgtddz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jwybqenb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uofnqvvx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lawrlpuu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tsrhjzbf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gnoibyyn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zwittrfz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqhmnehm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rqptagtw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hlsfvtwv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zdmqttby.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jrnurbzf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hdhfuisb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqbelypo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3plmebjrz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yawbxlkh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcpwawjd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3eimolalw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jbsnbmhr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jahxluxd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kmsbwpfr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nrckxung.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwxmlecv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yopysvri.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3axnfyqfl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iakvxctn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ilhfbuvk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvuhewmj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynfxmsrc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ihqbwdqs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qwgjjowe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwictjo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sradvdyg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hscgavdu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3alruqswl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bbcfgrdl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcftadus.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dyzyqznk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kmsienoj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3nebtktgh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rexrbhsk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qlekaktq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hcdzzkyl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3deftezrw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pgvrxjck.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xratyavt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yevypozx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jufsepmg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3yvcfrkhn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ebatgiha.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qxldknjo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hkrbgjrn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgqrqfok.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mhjlapkd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyiezzrw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zobfayij.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vdsmuatg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qywpahgn.html


<!-- 参考信息 -->