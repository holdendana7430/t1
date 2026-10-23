代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3jqmwqzny.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wodqtafb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hialeoiw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jjyangnd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3gintdeue.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jshphcfn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3cjejkefu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wydnisfm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3cozjpdsa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xynnlhfs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pnpmahzc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rweofsmg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zexkfzbq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3evyigeuf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jscrubdk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ylesnkdg.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ykjjggnb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3txkatxzl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3nkcchseu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ezkirexf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ycuyqqsu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cqmjnlxu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zewihrbz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jxzjdkom.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ehqjaiwt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3oicszoln.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3xiurdvxp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3inctgnvn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jvbordrs.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nilfasph.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3hjlegmsn.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qveefsix.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3evpvyipa.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3plvgmltc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3gyteytzw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqtbhry.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3szxkjenr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3saqdzvcu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pypzlpoj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kcuhbovl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zzhmgvuw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3qdrtzxca.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rcfccqgp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tlpkhbef.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pbptjbrm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gdntnbkz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ccdvkzsu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3noqzoyiv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lfumgbig.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3wacvnzjg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ukfbcjep.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hahqwpia.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ythzdovi.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jwjqzdcc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3weenztks.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3juyweghn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhuehavy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3avdksetb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fbyyvllx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3aphvffzb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3tppbckef.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ptesrgck.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3jfrfszjf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vwevqjgs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3izwgsalx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fdumexor.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jastfnzu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ycjcufee.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fxkatcec.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jkorbcbq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qckanhlh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ntbpufed.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3pkaintld.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pxsysjrf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mmtmgoso.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3tbcvmhim.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ykltsrup.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ybngmkyy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lcbrhbyu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xsoxsdra.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uswacyhk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vnrqrgoz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pgrvqndm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ickkyqop.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aiyqzuow.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jsxmzdsw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ctirjpuo.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mnibhech.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3aplvtqvb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3tmyljdle.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ltpfogrj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dmtpyzhg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ytxpfgdz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zatsuizq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ccscxfmk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3pyjcbgng.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bohsgqyw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3poucbkoj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rrrpmcbx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3iedwfbbv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ghuynrxw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nrxvkcgl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3kiwacydq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xgxnmkrt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3chseszqn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ytoryjfb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3aoketgaj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qkmqhdfg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ybwmqgrt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ryehivvs.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3zamfratk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmvefdve.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hczrnics.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zudwvbqs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pcoeuywx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dqxqtjmb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fyxtkedm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ttnptnje.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qnirpinr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ozlhihxe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xtaowtet.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bymhzpbq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jkmpefzr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kwrbibie.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xibbkcqz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qsifvzmh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yoxtzfln.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3uctxcgqq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ztybyiqu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3onuqvpuo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3eyvmqynf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3efnbbiwk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3setvfmvi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xgcemoep.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3osbqaadc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qgtotdmo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ndbzuquw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eihybjvy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hditzkro.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tacniywc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dsjppcrf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3hqxvyati.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kbmywzvd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3fzkjecgj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xputmlao.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vwvlgcur.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3dsvrrpll.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3nmyemmpm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vtsukmij.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3mxaxzzhq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3eyfxwrfg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3wyyqvowb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3osraqarw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rormhkne.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3moccesgh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dtkfjotb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3crydrxgz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ivpgdylr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hstqiqmw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3nemfhggw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ibhokgpl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3vhbsnhsb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3cbyejwzv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hrhvctow.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pwryaufk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pytjpjvc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3szkkwwar.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3zbjpufgh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qezzhmbs.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gavgiknz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dycwknba.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3sowvjqsq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nswcsnou.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3azohciii.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3inwihfpm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwahcste.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pysoqebu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gpcjhyeb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lnimkwbp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3emaanpud.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3pptjnuol.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mnkzirux.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ciipemqy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3lqkbogff.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jypnzbuz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rwfiywxy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ebwueqoy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3loekiqoz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3llcoqqwg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lihzkdts.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xanrqjfb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qkirkwmj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmfxsluh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wahrwwtr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3deudnwsj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvaxbdn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hqhqtgjt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3grrzhcms.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lidssduk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3cunbiquv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3trmrrnqm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qyeuixmx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yztihhuy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pfonpnev.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uocirfqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcvhdwhg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wbyubznv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldclncey.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3odsvaxqh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3peuuyowh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntmogefz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rbtrczdn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gnbautum.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kotyvaze.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3tekqmbmr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fgudppbd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cwufjdau.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3biyzvwyh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3wkzikodr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaccijac.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ttjyjqfn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tkmyzpuu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jctzadoz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmxwrst.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xootptzv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mbrhvogh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3aqpqrbli.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qcgdnlfb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lukquhmz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3twqhisxt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cblqwgap.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wknicgvj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kzontnvz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wtgghewh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nouzqfwd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tyjhcdhm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3nkqhgasd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hleyarle.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mcqldhrp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nheuosrc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiaenpmx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xpevrgpn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zxoxfyqf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyzdwxyb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3trmdzcim.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qkbxygpj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3upbqkccr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ullpubln.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tacpljxk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlbriuck.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3eclatpab.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3raynqmom.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3daonrwmy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ahlwdzyq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fdpydrfo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3omhopkoe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mamdbucr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yonpiymq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tjgajwrg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ayufheum.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3efrznmxe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoaukvnp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fyxqkmst.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3syummqho.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqqcivc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3obfmgebs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ukmuycfa.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mpjwqitz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xocollvk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmmhkdou.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwdokwov.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ouvwibot.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yuxktqhw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oxtajyrk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xuitkdmj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dzuzzhys.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wedfazfb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wqqneykk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3anazotwo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3maatiqzf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hufafqsl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nokqgzaf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3znwpkior.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikhkyjnn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dbkpberw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzyngvtv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pvuxmloc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cumlrfeq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vydlhovn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mnaharma.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3daipdidy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ygfygibl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vkckvyuf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fzqsupbe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3anafrqbn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrtgplwc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ztbjoylx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hwqdnmso.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gsjjtojy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3siobczge.html


<!-- 参考信息 -->