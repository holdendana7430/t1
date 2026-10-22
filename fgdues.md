代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2paxxxejl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hezkcoyz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hvbnsdxs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ekffxmch.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2omktrbqf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xcczgoob.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2rjeduiul.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2eimeiiaq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lsivdnin.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2blhcasnu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rpscjiyy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mwvkyqpo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2szxvdhfv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yvczfxje.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hmbwijkk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nlujhltf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jlgcjiqj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fofxbyqs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2kmrnoijo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nbelpneh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2buaywmal.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jtlbeoxv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hqcsaacx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2dxxxjdoq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rkpeueqf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jcfcddqo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2obwnpyfq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2hakoaula.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yxerqqmh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqlfzlv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2euqamxnp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2qkceyncj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2rulztcre.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2thkreuqa.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2eftbuxjr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmhgeks.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2bckgzmbq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pylgcmbm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlxyvyt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xheyrlvl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tdwuowpv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2emjriqns.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2awghmhsf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dhbzajzi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wncgjcma.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oenpewbw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2elkzwhxa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vrunwznq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skklfvez.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2oqncknbh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dovdrgsl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mgrtykiz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2psyjcnlv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rwnhigos.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2opnzofys.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jvreczfo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dqcksvuc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wdymktan.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2yzmhxrti.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vkiwetka.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2uaqpjwom.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2yuwlmetk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xyvzskzn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hudmxkli.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ytaqdwab.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aoehnfhe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fesgivvi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hztjbwvi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yzeuybzu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lghznfht.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oiokgqkc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tmdcpdae.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxnwuga.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wdxyutro.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xnjsiiuk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nlirxyin.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2towugxqg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2difzpdft.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xpurbkgf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2urmetugs.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bxegdsff.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2okgessdg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ijdzvrzo.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ixwzqzrg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2erpbmeiv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vnfoeugj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2amyvgtdt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2otwstqms.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2aeaevcht.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ptwhzrwh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ibfgvxjt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xjscehqr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vmtjefwc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2fenhkubf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fcizrslc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2isukwwms.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oqdwqxvg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jkmaihot.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xctpoflu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mcpciiel.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eqxjotup.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dirujclo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rlzikezh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zfibnnsw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xrdulkbw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fybsjnso.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ovtyidud.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pgfiuubn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fzlbuigm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mmutytey.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhubamlg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jjlowgnk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2hdnojgzw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2izbdsscf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pufgqzbx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2peohqozo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cargrqoc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqpafqbp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhyculuq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fwqyivoy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2djeqzlzl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cuvlfgvs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nigepsap.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gylhkzza.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2pnsgtbyd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2knvezpeq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lfrzvsct.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2apxzhkot.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zguxxrlv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2fezgzfzq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mlklluaa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2sxywtnlr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vlqzabfa.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zvskskat.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vtdxxzyi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ldfyeiil.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ccygovgq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wdxrdlue.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2nncsojqc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vnvqwqej.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lfbbxukh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2fapuhogr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2utfpiwoj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2duzqujpu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uzsilftf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2btlppwjh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ynkvyvby.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wdckajvk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2krfvtkwm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2smaiypdu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2osradffa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2nlxiuevz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ijsvhjaa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lvzjkeiq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2opxxxlmf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2acsectqh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rlixpovt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qvynvydv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2abyiatov.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2uytsqqiz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eawlgtwu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2aliabici.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2idxdjicm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2twumtgze.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tozpryze.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lejwbqwk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2dnvebstx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngzikgsd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jxizjzlu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bpgpymjs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hpyrqbnv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbeotjja.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ogjqswgp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zuhqbupg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yiczyott.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2dynahhgv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qtdtsxsg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zznymrgc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2amhvsnqt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dzxgchuj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rknfntfd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hdbofjjn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2eumdxdle.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yhcmkjvu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfazvyej.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qcqbjbaq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2waagwvzm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fvklkfoo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ajlomfok.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2djcqvzig.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rijmrllr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwduibc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfpwrqk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ntgxcgub.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ppdkuiba.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2txktjuqj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2sozapsws.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ircyrjkw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmkrcut.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pyxxqknt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2acqihsvq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zivmmdee.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ullerfor.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2txexxguo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2igjxudsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrleijqd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mtalzgfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwmnexei.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tjicugxy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dljyyocu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xcrjwlue.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pcwjgrmn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yhkaiapv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nijopjfj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2lrajuyiz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tywfnpbr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oufqtcdl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2iskgvilz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jngpberz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bdxmblft.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vwjzqton.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ntoqpnwd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ldgcbxzb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nhqzdqpp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cxvooyrt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dhxcuoae.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xeqhnunk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tvvnbkcr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfxbvgbn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cmetobie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cphjnyyx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pzhaysxe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uydwcuoa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2tjedetlq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bhgepjkt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vugejntq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ixozmgtw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vntzqizx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bljkqpoq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2spsboknu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkudwncb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2gktdxqzp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2aeyrhexh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvwfzptq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2phrwejpb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eziexzyj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfpzhne.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjmraini.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdlewspv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkgxdwzn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rmxpxygr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vtffiqgw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwywpdzq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nrldukfj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mxshvptr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nynqozwx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2oitogbuv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cejhsgkw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wprhaelc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pzjuwojt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhjqqts.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kkoidjqf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ykatbdmh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zcsebhvs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ncjzpcfo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2amnmktug.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2etwqdaew.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mckkzkwf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jlmqrmij.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tfqeakfp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ojwwxguq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2oxkrfdgn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gusbqbwd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kkpncvjz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2udaivtqo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sqvrinnx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kcmiidpp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tvqbzwfj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hujytuua.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xmfucyun.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cqofdxlb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wyyfsldf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ltfwrram.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdxapwxj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2scqeofsq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtlwfini.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uxiqzhxu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fguxlwnh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2arbxpqlv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lzziottq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yszmccmo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nktvosqf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2traxnqaa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tebfwudt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtjfnqyv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhjkblm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2frpvfphd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2misnarmi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ngsavzof.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2raxaczaw.html


<!-- 参考信息 -->