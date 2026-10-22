代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2yveilmcd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cshmprwt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2nwghhjfg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2slxbkrjp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sngmfdhj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2bbjezmfn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2omnasrbk.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2utbldtnr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrtawjf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ihrvdavs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sruzapda.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bnrrtftv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mygnxfos.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ohhbekmd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jxzyucuk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fviadykm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2rjxachiy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rswircpe.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2yukbhgnx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2krbgheuu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ylimqwdl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dwpwkupd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2krbfhrxn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2hygqliru.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nlwwwdus.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mhsbpxzd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vympmtge.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wbfdyqoi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eclvwnin.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mlznffai.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bhfnjhyy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hyirgxrv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zbmbzfmb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2twjiqvhz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2yfefdfuk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2kwjqcueb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2rsdnhwxj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2keoknpif.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qzeoppej.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rvxyxrws.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oohqtpdy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mjwtwehj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hcmrkuvg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vqkbqwrc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xvnidiam.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cyudyrvi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2awliflth.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kabxyegp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jtalgyzm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2unyoiliv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zjdypbnq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oqjttsiw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2uilzdroy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kknnrfrl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hqhflqks.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fangueuj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tauzoxsz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2kbwgkxlz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fgahgbty.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wdjbntjj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gzbmotah.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wvqcvhbx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dqowvbuv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ejksjqhc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2akurgcpi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2opckisqv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2iugrqyos.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rlqncwnf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2inafhnau.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2soxoyfie.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hviyivlc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2phjzylya.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wvhwjlve.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jiesfkyv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knpuhnnn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpthsidv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2arbfazjy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vfpviujr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zshmtqnf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2umaxswrg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qassyiqw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rhbfjjso.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgkhavex.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rmtribri.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pnoktixv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nigqwpqw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jrmvwpev.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gmeqdezs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zwpkmtvv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bpgegpbc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdvfevs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jstqztdt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2sifkqlcy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lvenzcfr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ngewpqvv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dmpmxjnt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pekglqov.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2gptckihe.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2znubzzgi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2xrkjzowu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tukyuvyv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dwuaangk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dcylpgkl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jeihqxte.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tqhreiyk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hfonxsxd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bqtockvp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2acabovgg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2cdaubvco.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2yvkuvfxp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2whlxvotn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2uvmeoods.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2hgydwqry.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2lgouiawn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ixsnucrn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qjojuorr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2jyviohup.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ykubgfpp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pkahumjs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwxtcfbh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gxsytzji.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eprwxbuz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2urzvdljt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2thhukhzz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jxeygoyf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzjdswi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zodlgcmz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rgdqzrqn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2srgjvzcm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pyaykakm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2trwnxnjt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nbrnjrvq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2yjmodbmf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nlzoiugc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2khmksvll.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rihhiich.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rwmnjzkr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uqpuwqhs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dsdygpxx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2afskhfxc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hqdkwqtl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2darqugvk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jntlaydd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2sdunwatk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbakgppg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qrncldxn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rqusenkl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2npxltpvc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfxeunj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2oltaxafa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pzvronnr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cpwemkjw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qqhojvni.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ysqysidu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ihvkopkf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ykqqhdex.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfbozxkh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wyjxjlox.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pymvvrzh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxnupuom.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zkjllihk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rhpmvecx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2sdadvetb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wuidcwec.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2idwnbrwb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmrcmsy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jougtsrs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vtxinwes.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tswlunqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eghyrpra.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hcjwuebb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfpvuxns.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qvmlmozh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wddoxwbb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlxwwlrn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ihilimur.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iwbkauut.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nrhymokf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uwohgqdx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mbuykhok.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xsivkhag.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2uggubmmx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xmyjlwat.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjtzfzac.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fzgjlpgr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hpopvstd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mxjdlrxf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hrqkynyb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2pkeqjpqf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qehegrjv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zzdljjog.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cewuwiph.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2avhwjeur.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2akieufts.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yibsxkqj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iikbiuxj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uybzqbnd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pneradom.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yaqzfswu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rhytjnqn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2buhikchg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vzxkvhis.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwsyadkq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddzcyhxi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hqzxknvc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zqeygzzs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2slqgggvd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nshleyzk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bdtxvisl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ekshmejp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2toaqzypk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mygjzfik.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2byuezhbi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2drtwsuej.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lewahrdn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kytargua.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jhdomfmm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dbkieslc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qpykzxjl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipxeubjd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmlgqst.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2htxyboyo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cfnisghx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zhlajfru.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lwkkfzcw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2srckhtag.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lgekqnkv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2abbysook.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2radbiwgq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmvaqnsf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hcfgprfr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uakswsxx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2oyshhicw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ccafgqse.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2smrtwksr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fvmhbbyk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jhefjmxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yrdfpywr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ksripvav.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2raxpubvg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yyhppksi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rsureete.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jzkesacx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2trybjyse.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tqkdrvbw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2iquxrvju.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xoyjdmtb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwlqrthu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2axftjojc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpehqfwc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2keucqhtm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qrivpbxd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bhsomjtq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gvzkbqof.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkqhudy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2sjheoawa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wbvpuvto.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uzxlwesf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgqeuhjz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ckbtdofv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rbqxignl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2oandsgik.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2fqkpxuzg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uezqiwvg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bqivsvgt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zatzdsil.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jkkoqkjo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nckutebq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pxmtoxwb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vljttutd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pvdpdroa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nibqiepl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cyvtwhog.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hdxgzkmz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pocagaso.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ghuhxhvu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mlojkubu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xujyleir.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vuzabldn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xfsvjfzw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xvuxqbze.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wdoyupxj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iculieba.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wyxyuzln.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpniemdz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eggxtbeo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2scgkskzx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2afqamsrs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bdzggtgp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ynunkata.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lpjidfla.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rvfirstv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mgnkkmzr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mzantxao.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkforxao.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2bvtgufob.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2awpbvdtp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2drrbzdhp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2shpyhxwu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cybkdbhg.html


<!-- 参考信息 -->