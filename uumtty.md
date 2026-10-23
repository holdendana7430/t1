代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gmxhoaea.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gmjzorad.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3llonrftu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3gymudgzc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yeqcatnn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yvpafncy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3lwygffsi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3avwyhbqs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ummuciol.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tcznpetl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kszffbbt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mxnhmqcw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gnhwqxgw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3djzmjvew.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zxizjzjq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cokgtfqk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hddptzjh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3pjgotyyu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ssbyrvkb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3afmmpxwu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3snrmymxv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lzmmioyt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fehptsak.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3btqwcupk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ztlxmdie.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qqyihxsn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uyumaqhk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rvzyksxp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oyapurqo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xnxiungn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpsptihf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3emzvnuqz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nxhdagle.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lydeuqod.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mjkxlrtk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jxtacked.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3eycmzmbf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mqslkaxu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3uyznvjfg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ijviuiuc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vcsursac.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jyrynsll.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcxvcta.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3bddtyzoa.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3odvyfzas.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjtkudl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zsedbbhy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ezmtdhog.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3qyjzthge.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dnegoaiq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3okdctkxv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3peqoeqvw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3sdjegmqu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3llhntelu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3hqlurnty.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uoieboii.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dncvjgqq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3zuoklalc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lszeujet.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3arqmuoxy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyqhfjyy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iormeqiu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ueyipolw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkxjqswf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxshverx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3aqfwiinv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3asriofgi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3snntoacy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3rykyrscp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzufgjy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vgnxthic.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bzqyhosh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3psgfozls.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wmmxobmk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3tqbydgpy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kjsekigp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3afwdaxxg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3lgoonxpw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aznqisbg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3imozjpyv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3daysqhoi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vldjvgqn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cahsghrs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3soxgxpuy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fcsndsog.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cvozgzof.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3naiitpua.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3vjmtvxvr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fhfwvtek.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jpwthbui.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pffrzqan.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rpxsxmxt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hzrioasy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xghpufwz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cpxaidce.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hmshtuby.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wqaluwrs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3awjgvfak.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3chisjemm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ihvpqclq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3thowkocs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sttpxtgz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ultcpwbl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mzkovsci.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3istiallf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3hcovgnvo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3raveaylo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qaawdhzs.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wdflggff.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mucsxbti.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3angbqtne.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3txqhbuvc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hyxdfams.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vtopafnk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zkgmyxdr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kdwjwthj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3awybmxyq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yfsorwqu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3jhbvvcdx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3mweedise.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3srejzwis.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kqeucaqc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3aaviygfl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xtvvztnn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3klksevjw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fwrivxny.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqbdkfwn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pddzgsrk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ukdzdacv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3furkfcqi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoxnpelu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3bkmjgmrf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bfybmfez.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nwbjgvnz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fgivqwww.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqxmodeb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3byhdzcyj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3adldwufn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wsdcpdoa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hlnppdkj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3akjoyahs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dvlxawfh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vsbvwuil.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3humekzsd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pblvxivs.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jkgkbgvr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ymifuxnf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pkjprjcq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3eurkbatn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3kezuwlod.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ucsickuq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3okpgvchu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uuauhjep.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lnyytdko.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3zbeieggm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wlzzmfna.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qaslqcys.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dbyejspe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3oesemdnt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hfolgwty.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gtyrzxhe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3tsplprzy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yrcvgvzm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jjcwxfqp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ezjosipe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tvylgtrv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dxeibpwc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fwfkccse.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3nkyxrwtl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cxuewmqa.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ydhitcwb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cdwamjjl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mhojsgdx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lpthslzr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iwcbyfuw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cnqlsrsg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3weehltmz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfuabedg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3abmjecph.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3daylbsrl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fohtqhmw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3cthsdpel.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjesaxor.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3hwdwjbxe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eqhucgrd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hdufzvyz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mlbyqnnb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ilqiywqv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ubiiargx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nclomnnx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hbozgvyt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3icoohpjs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tmonsoao.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3nfuvchtv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fodvgzwr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3eidonxjm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lvscszbe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oqwpiyih.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jdkooyoj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xyhxbqjh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkixvxgg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vzemkdjs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nprqzscf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pfmunbfe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3cnlspvfs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ihgqtmkp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3txomjfmw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bahjdokn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3okitjley.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xkmpdlog.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3iktvwnkj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vcoyqkas.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3snogjrch.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xmuixcwk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3crtsxuzj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ofrvgxug.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nssljpys.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hpkvcdzo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wdesqznw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bfhmtetx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ejecywoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufaugqhu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3chwhhvuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcmwsdxy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ymfnahrj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wpnmycrz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjsjwpqa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kmblfkfo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rdewuerf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rpidoxkg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjcmedoa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tqzfjddf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xmajdmsh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3uprgiwto.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dlromabe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhfqhga.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3prygtlwz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tycrqjif.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3elibrccu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gsftgpuw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hxmiycgu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3olxovwyb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ocpkgbmr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gygpxhkb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zlpfbnsc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqusxpq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csqpisxy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3khbjnnlc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rjdlwifv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3lwqgsrht.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zfsadpco.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hqubpxwe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ueoumbey.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhksbnrz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeunsgkr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3isyglyyp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3omvggmup.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nkshhddd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qrkhviuo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3izzwfovh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cqqjxugn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xpqqudqa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ianzleqt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yniacubk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdioiliu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcmhvzr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3niadpetm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3sprphauc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhslnzmc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3buxvvumb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3thcekynn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qnpqjelr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3azuwkled.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vimkdvsk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rugxhyoi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rzayauuc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ccxcfbqo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdsgjcem.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ahvgeqbq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bmvkmfey.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddufalax.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nihmzxqo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aispxohd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xqtbizal.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lgoqdrnp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xhkpxwuw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jndodxrg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jmzftebv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bkcgntww.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vlshmkvt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gbfmgtre.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sqgbvxiv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bharfiho.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jijvklss.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kdwllkgc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hjqrusnn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3trphjxft.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3clwopcab.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpxuvwyv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gmtgfgqf.html


<!-- 参考信息 -->