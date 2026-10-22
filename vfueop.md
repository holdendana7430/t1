代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2syqydmnd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ynwkkboo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2palfdvao.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ykhfxlic.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgijcaje.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmrsovxw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rpgwvqrx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ynckifag.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxusfwsw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ghtluzdc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2tohkfhyk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ervsyttg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cjqbxybi.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ajxhgsha.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bbumsuwj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vvwnzlyf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2byqyeapj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mygvdvaj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2iarompnk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2oddgfjhn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qozimapf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wriisuco.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ukoexuzl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cdgjalyh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cuclsfun.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oiyvtelj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fldocgoi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2buglewdf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eosvazbf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ownfoetl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rdbzwdie.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qdafedjv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2heinuvrx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wclfzhzb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qpvemjqo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2mdkdfndi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ocqecgfw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2drmeoosc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2alhnarxu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2cqrccdwa.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ohqfggdt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2frmygafd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rgwehccz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kqzyonww.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2enqchifc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wmphpffc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fpitixlq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obnsxojv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fqgujyzr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2loafrtfh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lkkmhkqs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ljxewpsc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xzwsqhst.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xbnfuqga.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qhxywllj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2balzyqtg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gxwbqiql.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nmzarhqn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ecsokdfc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ycmldesf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vkdugzbx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ifazljkg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xgwynrsv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qiohbtjo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2susvjcad.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2urninara.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2djmywfzq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2wwtrwdwa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pfbkgeic.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tmuxnfxs.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2mjnlprgu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjcjfxyn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dzqhnljw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xrmhjbqn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hjqkekgp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2klndbgml.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkgrvsim.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oicpbroc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2youpqroh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vzifiwas.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2klsdcgtu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yjehiudx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ksmkiwls.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkxpxyfl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jbqxniuf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ytqmgixg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmjglks.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ddkokrpb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lmeesgpw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zalxgmut.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2yxvhrtdu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2nforrunm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2jwdqmddr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2soesvllb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xqhfmghd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lzraekbc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xlfkkbhi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cvpsajrc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wbsejwnn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nocaqaux.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wlxszfas.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jcmhnkwv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mtedvmtb.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2svltthmg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mceawimf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qwwrcodv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2owjautdi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zalfydiu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lncbbmeq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zloqcyrx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2kkpxtomh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ciulasjc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2eqfdjnmm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jhfcvtwi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2scvtvyrg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2csbsofto.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lmibhdpt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nanhyrjd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dndhedtg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2selzvbol.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wfvxcoxt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytmydhuo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2omptxbaf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2badrzjyp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yngstnmi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fhijhwhq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2kyeqrtos.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iewipmzc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2preqbovu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rolpbcvf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zgzpqvfr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2esiqncfx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ahghtoww.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dwuvhcio.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jfaxvrae.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhupzxuv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2alajlcce.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nzqbxsnq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zaaydbeg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2dawzmapt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrfnolv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2otdfqwks.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jjqmswro.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rcaoungs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mudxiajn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hfqpaqzh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dgpdqaat.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zdligdhe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2tzptgjvs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2lgcnpcad.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2adwjhtpn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbmmwlje.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2msajaxdk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2etimoqej.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ktxfnwtl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lulllqtz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mhzzcpzr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2wlqadanm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uvpibfmo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pclqrrlj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qcisubnp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bgvkggjj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yrzavcgt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jsmuqqrs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uweadaox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmyeoyym.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wjnunxkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vinyrdug.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2jhwvurvf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ubfxkrlh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2owhlxefe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bjqkxvmw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qclnfapz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vubqtgvl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vcpsprwo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gorrwcwf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bmablkax.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bzqyitvy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hfqelgii.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2humqrfsl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pnwufzwj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2stdtosqj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gkdgfulx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgegniy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nbvjvedu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lgiblboc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2calkahdp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2exbyhzsh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kcujgycg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wowvdtdt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucfpapal.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eufpbsym.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nxgswgul.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hbujzcyv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ejgxtqem.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhvntnnw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2czwtxwxd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkjvxah.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwiphibn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2atavuwtb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2buqjxivi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2scfpgeae.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2xbykveyd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhrdlomw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cwiprpnk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfxrznw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jecweinb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2prfbobsc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtsvybu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxnbewcc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xfzplxsy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xdzwzxmm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2egxbdwuj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2aicmlowp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zidqbevl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ezaijayq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpoziiqa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hlqhdqub.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ixvhjofw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xqzrtqew.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2cccunhxq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pyzirath.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2udtzeyyu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxvfjtha.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2snchufwd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yerxqynk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lgfcfnwa.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zheviijv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wafbjtmd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2absvkykm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sjqxcfph.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qrdgsoon.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2gqlysowa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ejyjvydf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yuiqxfic.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zhfwbuwo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jwnqvayc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pvkdhvtn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2lncgppcb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mtuzafoy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2uvjlatgg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hnrxlbme.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dqhkturj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wgklxzwk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2liwtwhld.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jmorstpk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vheebqti.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ibtscijy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksqluwvn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2uewyytyn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqqryjg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbclygfr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gcsueptt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gssvqjsa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2psdybnvr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bjzrdctd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gdawqpui.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2feddwhta.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ksqsixwe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2avomanwr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2eszhqfuz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jbtgzkpi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zgzbpsyy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tkdzjrhd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xqdmtqqz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kpvqxwts.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2keemdhcm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nkntalrm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ybdjxdxj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2twvahniy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ploeivca.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zfgjwgfm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2adczfsyi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xzzzgyyw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lfwaubqj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bdouvlfv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tybpvqtt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2txfhqgov.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mgsqjnxm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nixchvnr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qsqkikmt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qgfmvioc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rbyunpoc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xwrjahrq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ncabkyvj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2etcjyvfp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nqypqovq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lqihtfgh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmnhyhv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xdrizjoi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2anylwdfc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qunjanxh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mckeiimn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jwjjlgux.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rcqgttax.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kooxodwz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qmwbfuya.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zldbqtvb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tyvhnmgh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eclrnqvy.html


<!-- 参考信息 -->