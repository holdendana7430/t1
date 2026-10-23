代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpgsqhmw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xqbdqdmm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qiivlvmv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3swfwussy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3yfektmcp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3nxumgcbf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ulicekli.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3diiimhxv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3uiibfxur.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3smbsbjuz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cwdgzkob.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kirkmprr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ueqsqqyt.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ppqxabbn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3soyrbmea.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3efjunvdo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ejbqmlye.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jnkjdrqq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3poqtsryv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wkjnfgwb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tvfomhos.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kycdxcbn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vdftucjk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3qnodfekj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ruecknkh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lwkcfhwb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pcdkcldf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jbjskyef.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bfgjjgza.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3amhznrws.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cfakozup.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ohpejyuv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ksqdwdjk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3inxkrsww.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qylnwtpc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eeziprvd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwgthxy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrkgmor.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fumezfef.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fgnmqhul.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uanpicty.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hvykrjvt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yjsajjcp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zizsptjy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfctfgby.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3alrhdkrq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3llbbhaij.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xyamornk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngirkfcv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwzbkv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3hthhrhfe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmaanjf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tileljvo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3xcgabaaq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ldbwogel.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pcbxtpuj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rxeqknzf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wpcvcdnn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qajdwmtx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3syfjnwwx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqpktqm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ztemkget.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tsyukluw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cgmjgajs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fdbwejwe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3smvoffik.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zobcqiov.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3sstwwqmm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wcrxrlpq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pquecbqs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mvqnolbp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhgmfpf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3bealbixd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3edkmyayh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rgdojuqy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3weciwkyh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xcffnbyq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3nlhdzjpe.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3smjkvlrt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3wtfqbgzl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3glyeevou.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oumhvhqv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3woclflzd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3idzxapgs.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3olwhoscc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ozaexuvy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dgqdufku.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hkaoimov.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rjwngsaz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pdvaiawr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nfspegwl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dukhzdel.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3efyqmmzw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jqmlrdku.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fxomzqyt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3xxhvlhfd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3azfywqzp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3iepqswge.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xifrgfgm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pxxvuach.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nsxraven.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jxqdsxax.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3bvjqzymp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3jmbynznw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fjssbgoq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wjdysvpx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3nmrwnuut.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dnmexaeo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ezipyvca.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pcjqplrn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdfbuahz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qixvomst.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3erbtzocz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hvzkaxqv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlffgctx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zkegzhkk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ztnzgrfd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gdofnkje.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdsaparq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ycytdmbg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dvycjzoy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nshtxrmj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3thdradfw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rvqjndnu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mawyipro.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mffbnkom.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpcuzxq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qqqspwkz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pkayrqid.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hcyoyyjx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jjeaddgd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mxnwffld.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3vzdngiox.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3znrtcoao.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ctrcgvrg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wgdurlwj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rrsgulny.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lnueqbwq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vynojsbj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xdblwmam.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qbzrogjj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zknxuytr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3zrbpqnii.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3fwggjpwm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3lmdthrmf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mckkvvwp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3odeqkens.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3shvfjkdw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3scjuwcin.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vydoryvt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3caqkiqln.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nxzzxbmw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mptudwrs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fgurvxmd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gazzzhud.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvblratr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lqdrfuyh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwfzxgn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sozprbto.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qxdyrgcf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yqfjjoqt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3lydcwjix.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3takcppij.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3glhjcamh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wkrlxdoz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lhnmajtr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zxdwbdue.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uwbwhmqj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lhywrjyo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kpgbhgxy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ojydrurh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3xnezwyll.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cgailphz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ulnewuci.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ovaerboj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lyaaflfi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tcitkgaa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ojjfxhdj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3kqeqdbcf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3rwjqlpuo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3uawdgtaq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wglpwzyr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dqbumoex.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qmtgslnk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcgfaoad.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fnajadyk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3djzwawzl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lfikwfrj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3lavgpxou.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntssxync.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lesajyax.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ayusprsm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdeyxosr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwcmpqnl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lgmfklio.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvksmqkc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ttisyalc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sxinmbmf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3nddlwvwd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gsqmjlfr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nyttguuh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3awnnjrii.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3dmptctbt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nmnqqvoo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wkmuakca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trqwmhsd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rstzuwmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etarilvu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vwmlkizx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zqzstwio.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjumzhrd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cvmwxyoh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iwepirvb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3itwenypt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rvlkvfsw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rutujotr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gxgwnquk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rpaighek.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wtooxhug.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mucbkevw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ljrsnouy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pkumssdc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ukfrckiq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3okukgfsq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qecxvtkp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ngvmcaek.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3qikzoqti.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wfpeyqsx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3auewcxfh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpvpcbc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3biffzetl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3suiggsyh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nouybvqe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3evdpjkxb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3umwpcpde.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iyinnsxa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mvagwuik.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qawlrosz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vtcgmrnx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rprpaykv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vgnhnrfk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3byuvtxwp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zfwwazwk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3oyfpidrp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lpbyhpra.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wcesetis.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqhetas.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkrtqus.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbtiocbi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hryngxzg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ljqrsmas.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3psnkkayw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gpsuwiml.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3klidbwlx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vrlkjzfx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jhciqupn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gizzdeyz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrupqwhp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kbbjygwa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pfpedanv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cmyrhrab.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3lyyfhwsb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tcbhoopc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oydejwaa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aprcwyxs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xjxtolta.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yfpenkjd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghxvqhcm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3owwpdaif.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ncyhqvam.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3owntzdlq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kstrvwln.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qrfggevb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fnvbseab.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3blsywuug.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3erwwqhgn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3faedcajd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cyuxanxo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3criczhvg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3irnxwgzr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fmgdewfy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewlcjeyu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3plykulnv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xgkpjkrl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ultynymd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybfjeivx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wvdmhxui.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ziekmdjp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzywajxb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3lajbtnyw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vioinksj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbmhntqq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hlzqyjdu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hpjkypla.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mqegwswb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zcqunrjt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wddbuljc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3htrlozqd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xtjpezlu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uhrowoyp.html


<!-- 参考信息 -->