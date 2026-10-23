代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmfwinqh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3bgbujpkm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3snkysxvi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3toadorqk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3krxjknxs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3bdzpjaum.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qgebeyun.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ccgeakjd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ynlydugw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ubmgqgmf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jyyuhaev.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3dcpjgsoe.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3zrzhfuut.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3foocivyz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vvuobrht.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xfviwkol.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3brkecstl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3svyyywpi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3glbpyixw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ycltjbuo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ebfsocuu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3srwucupd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3kwcnlzvn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ckkbghzw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxyascz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3whsjyrmb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rzeoezdd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3noimtooh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wprrjutj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mtzkvaeb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3cmazyujg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3yehbgkss.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bvhylstm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hcqcfuts.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3shxcsbku.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qlyhpxbp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sedfsgks.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fpqrdxgh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hakiqcqg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mrvxvhak.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3twfgyenm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nclphons.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kecsrjzi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eozgcrjw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tyibfshn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3dhgrtztj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kxzjpcwk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lfycitef.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wasdfxzi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qpjsooae.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fkrruaoc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3absxgkkh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pqhrozya.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3elebmtxp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zufduuym.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jlrsnlle.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ectjdhhh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ooclktnz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ibrpucvc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fwozihrq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3vjldupde.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3iugkebub.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnxvcfqi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qawdjswp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3esaldqbq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3viclpbwv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qgdqkcnc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3taybcpsi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wnysejxo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3itcwtnev.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lqorfieb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpwepwlf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnltongb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3skjztipq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pnbzwpwc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3adsljwdj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vnueocct.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jcdcjtbx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zxfnzqzs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wkbdemsl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wemktisj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3nmtusgpo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3secwvavq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3zjonchqc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qmbhrblz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3hyzteimk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qhjwottw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3akfejjpi.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3umdjdwqq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tsjwerra.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ujxfuujy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fhzuasmr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3harcjznw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3yvghmitj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mnjnylmj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3riihsjrp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xfjnhuxa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fwtwvkid.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kmqapvoc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hukcuuqr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qamrjjim.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yycvkvue.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wagsdgqo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3aopgnlna.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3hzvatvgx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3golzzvsx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3orvcaqxh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezporjao.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxkpcfn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3karnxzlp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vzukrfez.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wxsxjgxf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3liqutjco.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3aqehzimw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3zqstnyug.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3asbgqbao.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3spzhthhc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ivgefgfd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iawkibgr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wsmyspog.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3okbzhxdu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ojnypxel.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3vyzwjtag.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3rngdavrx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zycgxwrg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3neabdcsf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hixqfxlu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3uflzfncy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hgwuymlo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ocyqqkxu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3acugnrma.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lqicclyq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jrthppxx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3drrprhkw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zwhjyrrc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3htusjntm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ooiihlfl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qlydpeut.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gdhreeou.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wphdgdlo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3sqtqecky.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tiiyxpao.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzvjrjle.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqdtgkj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubsskihu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddowrgbi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ochvgids.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdyvjxt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3llydxehy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3thtqfxtx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mmgsnutc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jhvjbblt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3hiqzfpuc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mqsuwgfp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xgwlkhnh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3akhwxbla.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3sahzajze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyhnnkbs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tjpghygd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bumvotyu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jjpgpmzm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3nlqcwfpj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tlwmhlni.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eyupwpsp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hdknawmc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3flpopdxz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbmbeopv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lrajpism.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xybzeusm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3umkpjaab.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kifkcvqh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjyqqsjh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pskgvlvr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3znlsmxtq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gutztvwg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbykebp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jvsjinaz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3waxfywju.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3whrhtbgx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vgonpjlm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxwrxpun.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shpvpott.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ybnsemkg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytdyviyr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zmmwvasp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yxypvhws.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vvybbmig.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpzmaqgz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gjqhokrc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3oyyukglu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nefbgaum.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tcsrddvi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qshscwdh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xmcyaugu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ajomftuq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdhjkobg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jxydpuwq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fwhabtxr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aefvitsh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbrdvzt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zddgvbuv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcqbzyac.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kjxjilvv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3usfagnih.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrcaqxan.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3apcwqnht.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3effdqumy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwalflra.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sebmhtzx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnizdbvj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wkvkuaeh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3upixdkcs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwbhdqzb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3epgnetgz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qbzuydbl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3whxdypho.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jajpmqui.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yhiejpqg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqjesxja.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjacvyki.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dilqmcyp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mdwqqplw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3miecfmli.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kvfwrcne.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3agbwlmzc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bnrmlmqo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xisayzzi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3chjicscn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kcydoqcc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uwrkrzyl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gxhlkyko.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lfyrqfpq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vtllbidz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qglybdgl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwtgsrdk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xsggexhc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3epfqekwd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yilftrom.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zjbfhsdw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3onjyskat.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lploxgee.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vnewiutz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wnpzjrfl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eaislnev.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bkhnumpd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cgxklroq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3buwzhkvq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvlfppst.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3aarqjtio.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3niggtszo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hkhnejby.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nqhwmhnm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzfzhtn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uzclqskt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ulsjumvm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dvesvodo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3blavpmdr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3yuntuzyq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fojgcfya.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kmdeonlm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ovuyyuba.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tiuckbia.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vgmfprcv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hwlbnlsx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bwppbamf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhbgkcdq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qjniplrk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qyaoiynx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3thdlhcwx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xhkbhkps.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tmqbjaaq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dunvasby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibjubger.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jzndhcnq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3rbuumndn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cvehscgs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ypqyzugt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3shgatgtt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ffjqqmsh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzsajdk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tuwtstqm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsegkqko.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dwlogwgj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kqnffett.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wsmxemab.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbzwzulo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lvxoshsd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xemosqir.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3msndpvme.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fvztwkga.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mvnllsxr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nrmitdtg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3znaufyqp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3txnytlhy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vekaauvo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fxdoqsvt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dpwnmuhw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mutopngi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qfrckozz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ztibvobt.html


<!-- 参考信息 -->