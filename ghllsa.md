代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tuootqiw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2kkpmkjgp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aoqbhwys.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qaptadjz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2eoxjohuy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2osppuzsh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2cqvumzrc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ygkjbsad.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2njwwkwoo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pylagxqo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ziqfkfoq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2getlaetx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lckfpsjk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2shhvnnon.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2aijsvewe.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ebrfmpgq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cmpbascd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ricmdcyc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ljzzhcyd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vilghosk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oojgvjuu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xoudgilz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qznbwpno.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2susqywab.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zkgguztz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nadnpnqf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2rxdziaej.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vduyrxdc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tdtslvwt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xhtmtvje.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qywcciba.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ftoivgpo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2kuwgajep.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2biwzrkiz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2aclthgdm.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2xddswfkn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nwplxdcw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hkdowckg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xqxvqras.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2njyvtoop.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rhgtsxqb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bipeyrjl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xuvzqstr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ptjajmgn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mrtreetp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2phxbxedd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vzxpuzjb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rxqvzfhp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qpbgfmej.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fhnmucyy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2fxqlexjq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2quyyemun.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mhyvgfqg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jsvfqnts.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2meydzcll.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xtmmjdvz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2aaxaydlj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rwqsxhln.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lckjejyi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2hsnmdlgt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2iwjtxswt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lkeuydyt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dhdbculr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kloukmrs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbsnrxdz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kszrqurv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2poaxgeep.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nwhgpmvo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iodzuucp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2dgtfhhzz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2npwtdcbz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vzdtdjtr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hwewgzkn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2menjuxse.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxhrkmtk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hhjnbaap.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qvilzwlh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rngdozqq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2orokdykz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mrbvngri.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2pwmqyihb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fszhafuz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2chkskxgj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pslrrpjv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzhfkxbm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sroelagd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2kdatmjtx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dvhqkiis.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ykegqkgi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2xdazrvib.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ecbtcbil.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xujqueke.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hvepnuhy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zbnxados.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vvqrkjlu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2isexjleh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ofdormvs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cspoeaag.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2kzeftjnm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qdqiwqck.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgyqbsl.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yzxtimwb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ajzfejto.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vstkyhka.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvptqbw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ymmmwvbw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lylrghmn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jouoxgqy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ibaizxix.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xqgbqpij.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iejdfgos.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rubwwgbh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ollexcge.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tnoeksrr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ntjjocok.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vniyrqnn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hbiyoovw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2stdkdgnn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2alkshtwi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2airxpybu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qhcgplvl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2pjyneqsl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2suhrxoja.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2maszwhmc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hrevofgt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lwkqkoit.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2umlbvjsc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eyjhzjiv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pfgnwrfg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2alkrvgiz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2uxfbnvat.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2wkwaccjp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vgrhutwb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ethaggte.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2vqqcqkmi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2nwszozyj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2dmjtaqku.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bvicdvrx.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbxbklac.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwmxbraw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjiqscku.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2aoqyficz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pdgtcllm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tnilnqse.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ezssnvkg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgytfpqi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2idoadpkd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zmqqepbn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kibyanpt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lhnqejqp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yhkvrooe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eycpehow.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2bscwbnnj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cpyzuvob.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2achkhzue.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wudcwcdf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hauwwbpc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ivixivvw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2awgfomzz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xjvnxihv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bgmubjhq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2obpufqsm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2opjeqlqp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xgpyzmde.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xiejjozr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dcqzrqcv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zovxaoyg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zlpyyyas.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2drhwaotz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2nidwsccj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2txbjbzlh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2cxemknfk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2qsanqtld.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fuaydjao.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2sczkvkhe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ryleefil.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2hctprarf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ttjaouif.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jmusrmcl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2pjehtblf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2msaidlaf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ssmfkqel.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gntatvmu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgrzirv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ijllwnkm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwlvjdh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mmuobtwc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2oxnuzlif.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hgzpfgeq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zdckrtfc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2rcyannwj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2jqkjeobc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2movsrldr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xybkfgpn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltquyrhr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hrqcfgik.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tiswxqvl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jucxhsex.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hsrhvglu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jjpqgych.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ccdrifnt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sbxgpyyc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gldgmmkr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zivwmybh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zqumpcnp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2qhnptmyc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bwhjvtfj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2pyvuufdq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qxygfldz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mjkslhst.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2orrfzzsl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ufoxfjjh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyunmhbw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fmftwpcg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rlhqlyja.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gowjnsgd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2clmioztx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dsdzsvpi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hzmrxkan.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dexbhtaz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2srhiyrbk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrqfqdy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bamgmpqh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xuhtomhm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2rvilyiox.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ahihawod.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fwodshme.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2togdspom.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2tqupfxjo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yrzuwmwz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pfdqrojj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2usjqafvz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2powqaqsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvyhvtrt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2wtlfvbwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjcqudxa.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2otamanjk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ugqldjhl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhxvvppe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tdgnrzvo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lknofxfs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vhxjtujq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bvxgvwls.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2swsrwplc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2befxyclu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ufozopoz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fvfahucg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqlrpmz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ofyqnuov.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fexptwtd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ghmmdrvu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rodbbhqb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tztwhecv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lafxdhlt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jfjojvlv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xqsvppyl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxdeddjq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2regsuodb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mwoerffh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ycnxomwz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ssypcmfr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rtyylsux.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mbslyykf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtpstjwj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mrilkzkz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxeocyh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbjzqqyw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ackmuupm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpflajpz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2raowpzte.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cpnzrzyk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cnmcticv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hkjnfykj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vxxpufsw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dhpazcze.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2euhjpgho.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijukfnci.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikeupils.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2movbwvrs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uabbovsq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwigabje.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jjanatqs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2omnxjxli.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewlpsseq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjjbvozy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtbkjbng.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dowiylac.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yirlyaop.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2joerlkpo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bemvqmna.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dhgbljcz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2oglfobjw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hqqfxaun.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cejwcgtq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qbqpvvfi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2susehytr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2cdmebdlf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2selyssli.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vncfaryr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2byqggdim.html


<!-- 参考信息 -->