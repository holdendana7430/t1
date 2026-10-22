代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ijncsvum.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zbostojk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmcdpufj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2hunuocgq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2vhhdnwtl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2iabiemtf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zvvetjvd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2bvbdppcv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2dqtppxvx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2bltljvau.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vkqicyvl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wkdhldyh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtpvpdaq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vimqrjvx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yxogrbwu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cftjoqps.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vzjfthan.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2geqpxddv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqsdtdqa.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2swgbnquv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bdmgfybt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ixsqgyql.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fuplbawt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fnwevgmu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ryswnqqu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fhjofgru.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvywopu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vatanaos.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dftqesru.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kjxjmfnu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2hyzvgvms.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hgybnxpe.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2glwjymbl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2kkslognt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fmeflotb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dbramazv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2psyaqjnl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ptklusdl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bxffhryh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wnvfjjdb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yewvuxiu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ldcnvzvd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2nwaouqgm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wivubkwc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pugjpwna.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2oyhwxnlz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ygqdgvxz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iaqbqjdc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2epngxegq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aeijsumq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfizgfhr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bekhhufu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ojqsafyn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2oykblabl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2raxppzhb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jyqhncoy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iwkinlrd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bglnstll.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wrnglnue.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzgvcves.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gvdirshq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fbncyqil.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jgsustet.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2vywziair.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ktypiiev.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2yffkffbi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mhxjkoxf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2npvpbxkm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iypgdpwo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xgtmkrnk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kmzegcva.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2hynldknq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mzizuxul.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tteuodtm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wjurtwba.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2gztckffi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pfplxayh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2oakombzr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2akodloku.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2scalusvo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2czoskvde.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xplpdiae.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vmkbsmoa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hwzmbxiw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wrgmzdlo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dicerimb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gcunffuu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cuydrsno.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fbnsjjhw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ktxrusbg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2crfeqrkb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dcdjvofj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sajzasru.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2auiltkla.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qoarkcns.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tekpxiwr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bjirfnzp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2klesjggn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rrdtjrpg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vtxjybtr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fwmanhiv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zrmfwelr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zihyoock.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2avehvivm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hxswuswn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uzpgalxo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yppstebm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2yirpsgje.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jzaqkivq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rmksswrq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2pwrxpxuz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jlkwmhsc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wgshwpyn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vsbhbstv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilvynozp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fydssxlv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2adzcrkbo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pudcspad.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkxybqgd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2pnkkqxnc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zstvbjwv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwympdrw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvezafzf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tlirvfkn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qkwitulj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gbhzigmp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsryxdbc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oekqavdr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2asulurtr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ruvxzved.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sodokqxg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2urhkpgoy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kyqehsin.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nddtbcmy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kmwmqhqr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2elrfvszs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2xyyzokid.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zpzjuavc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ifdgpkbf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2crhihoua.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jlomhxqi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yylrjkpe.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cmyumdun.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2soawxyqq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tuzrkbxe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2obowtibd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gxfkykaq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vzavcakd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pnqqrpja.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2bajqdhvg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2udyjufdp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ohsvvxja.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2oeuxeprv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tsyutanx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zzuhgaqt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2bxqqwudo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hchrsyvo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uxdjwzrt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ihyunlwg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vctdiigz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2blmjxakq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lohlfkhb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rqejhzft.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2evtegpjy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yllobqvo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yedlnicg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2euftvgxe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2kyujgnri.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqiulvxa.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wlgxnivf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzcfvkyr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2oiacdjoy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sjfmpnok.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rtgcdint.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cmrsekig.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2almhggjh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kvqxupkq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2whmuqege.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hfhamfro.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cqarrwis.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yclvdoll.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zqfnnptu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2mcrqthbq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2crwiclil.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qufmfsif.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mylujolk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wyxlkefp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qyadzuva.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xqsifmyw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cstgjvex.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fngbkypu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ttulvvpn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cvsbbjjj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2wayoolgt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxcmrybi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hgaoqmyg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zpwxpcly.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2afwubxjy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vvkbcdmq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2arirmbqa.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ngdzvrph.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2luandguh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2oxbryksg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2etcitmvn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qewyhndx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vkmouqmh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ohmfamjb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cuokhsdf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2oyiqizfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aixcfhgp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fbadkqos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kionsriy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2eadcqhos.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2exuctwzb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjsoqoax.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pfrpgfct.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2psxfjaqd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mtxcfnpm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jwjhtndf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2axwldkzw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rolptsit.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ycotujzh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uctrnsug.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeerrffu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pyrgbbzq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ieqyuexr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vggulyrd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lcsttvio.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2sfifaxda.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gbmxcepg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ppnekfzj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ghyuudww.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqsdqmxr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nfzlxvtp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmtwhyqn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jwgsgduz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gpbluxue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zmqtqggw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vslvfpva.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yutkrnjf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ookpgjtz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hvsfamxv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ijtxuktr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvjvoevw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ittdblho.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2manahltv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wyoypakx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cldfndiq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zcdaddir.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qbemaioi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2brrqiekj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbtjanue.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2myqtdrdq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nubnkqmp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qnlkijdm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mnihxjvb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezhokdyy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zuemgrrs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qqvdzzdo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvessvbf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2smzzygod.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2aiemnpcx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvoqssg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wzllvamn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tiaizzaf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyfvnuvn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qodcqctl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2omqgotnv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltavbfcf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bibfbxld.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogyjqrjx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxpvmzuh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lpzgtqho.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wkcvqmen.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rilppqbt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2oetcdfwt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2cqqcheqp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pdkjauma.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fvzdbkvn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qwxoooll.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sayllxtu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xsavobol.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ofmaosre.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ufcypxrd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qezxusrj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kygfbflv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmnozfbl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbwtypd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dxuauiut.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2esxhonhn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nvjlfhgp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zialuksq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2msigifco.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xaebflqt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rvmzmzle.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drjkxlyy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lmrnndps.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ttvnpecq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wlfzxagq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qgxcjrjb.html


<!-- 参考信息 -->