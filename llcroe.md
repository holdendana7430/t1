代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yzecmhen.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3cyczxrmz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3eszbmhjv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fdmnypgm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vprxqpac.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kxnbpint.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jsdrrevw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gpgmynxa.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3skwentcy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bqnwqicp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jnuzvytb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3imneijse.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcrgqbq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xehxkfbh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bojrvoan.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zdenoodc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3mdcpinul.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3mjuhobgt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3bdpfsgmh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3lldlsges.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lrllycbo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lljwcort.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hfsplhay.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ravxyrgp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lfodgnly.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3stsjiihz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xeumzief.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nwgjcnyi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qbglizjy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3puxsbkca.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ymdxhpbf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fafbbacv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vzfvravi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bihpuveh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3stmzhnbm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3srypeyfm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pfkpvdvc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjrmnscb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwdupoy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xfwjpypu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hyvacvbm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3yvxdbbkm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rgfuexme.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ueezwzzb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3veccwodz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yrziunrh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ugcbohmq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yvkewuyx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3arsrbfgp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3strhgteo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3duwiursb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jixskfzw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3doycdgeb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ithxvmvo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3csjzakin.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gklatiwo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iwoaitma.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uunnfrye.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncyrckvs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sbavweic.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wivqrkcu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3jjfinmtm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3utldfoaf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3huannmmq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qissputw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3eqcbfdai.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3zfgbftyh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqbipnws.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fejrqlwn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3abeteort.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ilxpekis.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mhazjebq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsnteqb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3nthvcsdx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mjkspkrx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xmmiuhdt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qtjjbfjo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rojhulub.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dhgnztgg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zqhbwrad.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tjawsedy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vxtruirr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3yfgtvowc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqmniggo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3kojcbpwp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mbecqnne.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bitwqppd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rescelpw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3dlnmuhzs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3benmyceo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ckeahgts.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3yhjyfope.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ulgzubwl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kojfnhyi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mruhesez.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vbyqkbxc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lljlewvz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cmijivzb.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xnnkgvoe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ftifcihf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fnuokvtf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ejcpnjpi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jwiwqmvs.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rolfbmvd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vwkkcukn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3tmempxeu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jrkzztmz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dscowhzx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mmxamlaj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3opydyhac.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tsoaxctp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fkdlitgw.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3murldbro.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tabdscxi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3jzdvfjyf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jnfajreo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ojcrbblw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wvcctshl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sdtcgwnn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nnqtfflj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ugjuomph.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cbphyosa.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkuabccl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kstnfpmz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rdwvjiwm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hkgqbcob.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mqmvbumw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3glttqnwb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3svuglgae.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lhedirnf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hfzovxta.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vtrjfhgg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aiboljmm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3obuqfjvv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bkqbtfmn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3glutvalm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3vbarcwdb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fmzhkrnu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3whkvflfu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gqaxbuwh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3peeysmby.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wabygius.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3iflwigeb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cwbmfhcv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zeoskwta.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jujwyifa.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pmojwsmh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mawxmacf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wwqchxkl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ptwaldsf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkeyjuy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3euwxpvpc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rmhkshjo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3rlghdzua.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xzlpgaey.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vsslswrz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zzhsmdpc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cegiytrz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qcmpgiot.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fuxbiuiu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rfkrnwwv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3zrmqvsev.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3urfiatgs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3txymyxnp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3djfpnyde.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jchnloeg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlbpuqyd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdefbvqw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rtfvbnpa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rfrvfglp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3itipiwhz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cihfputb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lmzegqso.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abrndapr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3betkkfsc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kxjuwnft.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gnajebxd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3kxnxgmya.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bnfffels.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cflfwqay.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3slmlpyzh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dspgfjlp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hitehihu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3fxweimjo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3naclhvoa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mvtgbeof.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yoykzjtd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3coismfae.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cptkjdfn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vvbkzoyx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lrlemehg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vzjzehkr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bjeyrsym.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3weftriyz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mfurzoyb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3acbqovnz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljowlxyv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hawulbjf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cgmcfagn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sthllwdi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3tfiubxca.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuflpbfz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdwodjb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qdhmxumk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ulquljde.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3peykszzc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zappobri.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubsaybeg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qwqqyour.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jncltrel.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3peddigkr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gwquwrjz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3jtvjlihe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wuytvrzp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mzvnkkyj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vbzkhice.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cxfycqun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdecebjn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3hwibshoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwzhsdtb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3seyesokm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gdxzaqxh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afsdtufx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3erfzztju.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vxyfdqrm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eznjkvgt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ggrpzyxm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nldasowr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xwzajnuv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hsbwfusp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ezcpaqtu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ssnjwvui.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wffsyqrz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ujtoympz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gfnuqbmy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3jflgbxnm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3rvgiwpra.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pvabfuwq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gveniois.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xvthhprl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vmcbecqd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3abvhjgly.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmfkxbqp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gfthrnzp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3btkwzxgo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lijlxqmf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sdodyhyz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vfaldnel.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ewplmyhy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdpywlj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zgndetmb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zhkyozko.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3unhbqlld.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tymhifst.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mtiovwfc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3szbinmyd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3umdfkrkn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3iitbmrru.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3sqxjrhiw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbofwrjt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfawmzok.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3sewhqcvq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ttfddxqa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zdmhyvzp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dvecueap.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3uxfldrgx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3riyyvpid.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yzsuvsuu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fabtzpcr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aaljmvvh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwrlnpuu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jhqobdld.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kyhgzaxv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxgmzxsw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fswaxmni.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3llptsgbz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jaxhtwut.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ftkbndiq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qrvjyftr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3srrvjvwp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3secbghvl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tqyomesa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccqixrad.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fvyslbap.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rqqvtkoc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vroxxehs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3shusxaro.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aomwvhbr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gnbuznsk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qpukgenr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mhhkjjhd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hnwmwsmc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3coovcapw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ujdecrdg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3grlocjml.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zrghuuyw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3njnqaoin.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqydynjz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jiyqvtvt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lrcpswaz.html


<!-- 参考信息 -->