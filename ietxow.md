代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zwexpvee.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ccvkpmta.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vkugaozp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlnjgjw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3dlutlkca.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3oilemfhf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rwhnsyjf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kdajpzhj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mmfkddhp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tbveedna.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wcsjjizl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vuwiaeri.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3amlerhng.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kekrxwbb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hzevimjc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3nuwvqlta.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tbxgsbpb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ywylipvo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qpsqeobx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3kzopxzfu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3sdsopxmo.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3flvnvybb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mslcrhbs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xftmempm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3znktrpia.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tiadmgif.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3msbpyprn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hjqlmffd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fsoanhby.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rtkzjuzz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jihveuno.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fznlyhok.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ogntpkte.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ygrbgjlc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3snozcyag.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3assrntzg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wojqbhjp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3uwedejtk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ofqswvwp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vfffpfxr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lznxzver.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cwnkiznn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3slsrhfet.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sjyhbqbj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rjjeesly.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sknlnrcl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3farddovg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3oyffgmcd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jxhaalsu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3khxzrkme.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3zoqwhrrc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rjaolbzu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3cishjjru.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kfbuhpoj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztoaxhnv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ysvbdvud.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3utydpclr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vcqptqeb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3royuscbz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zrwwuwfw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bqotrrmz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3annxpcaj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnnidhvm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nsxkdqvi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oizppywl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yncbyttj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ndlcwlqy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrvuzdqe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nwjtrusz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ivmyqgxr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gyqncaex.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hrxjscwx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fhblcwnv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3zazvzckd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xzbxjlgt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xantnqhs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qgtbyong.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3haubntgu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ptoqzans.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3rxybetew.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fndsyazi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vhptmrfj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3aoplvdhq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bchqhgxa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dzbbztha.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ldmvwvlg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qrivsoar.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hkmlewvo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3unysquol.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hzvhupko.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yzmmsumn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3atzyidqe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gvovnign.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tcqhgrds.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3cicgrbcs.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3edzrwxzz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3uzwrmvmi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gzplymme.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3erqyepcm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rwivpvmj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rljpwesn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3akvukstn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3enqkdiwy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zpehhmcr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qgbxorzp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hdeqlwsx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vqjcrtms.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3clzuylxa.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nmjzxrru.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vafhbvgc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxwrfljx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gtznbypu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bhupyvmf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rbrccwzi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ixdgrgtt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bawprfwc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mkjpvywk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ffpgzzwa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qvwzvvor.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itvkfjdr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tflkaogg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tvrqifry.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zsfzzsir.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3msnxetos.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bxcnrbvr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fipzlvjx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mjjeldvw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3pfhgpzrg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3iuuijzlr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jjtkptds.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlaovxjg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fhnrwfcf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3tqfizdez.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fejgdapa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tejohnth.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycylufry.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qacduniq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vlmvtfoq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ipcuialg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ifsyfacv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ypaxuzql.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3arnkeuyq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3usmcoxds.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wegsvwfe.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dneokgex.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tngujubt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vdxqiupq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wtfccjds.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xutfjkgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrlczqgf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xgkkybns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eszpolcp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3paorsbbx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3mkmblwcq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mblddvbt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dbcqairf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fllyfynk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yzhipkdf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ykfhtrwi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gjqtjgbf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3begpbafv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ciwcgnxu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3honsvkmv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzykkxre.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qdliehxg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tkbrtrad.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jsiupjjm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mvzxvnon.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3usheccsz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dxisfwzp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lcwodswh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ncfcskas.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xismzuxi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctcqulnz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hzuhwizj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iqxuxqqn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ogtzmaxi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uqejdgvp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ffwkuyxr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ecqdvtvd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3beszccuj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3humxuhyp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ocukfofw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ygpytihm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wyhemehm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xbiekmai.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jnyaumwq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3idnxxtqv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnfoipyw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pczwjhro.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ivwqroqz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zbjmjgqk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbalzodl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqclwucw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3knezvvlc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3fmwivjxc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxldmozh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3prfmuhwh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3iyeulvws.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ffzpnbpx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fogyhcur.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ijkrxhnv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzdqvrkn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfvluyys.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wokbadfm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ktyapbci.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nnompqrv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lfrymfrd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkimwxgh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bekwqzlp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hnouxcca.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3akhvveeo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3agmrayxp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwzmppkq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnzihqqy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3giykpbvv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kzvqbnuz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mavevvhj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sntwrniq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3glnwhuuy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xnoremph.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mwyydtqx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3pyhscdle.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhlkewk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yihvpvgw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fxrmhijk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzbchgpt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hfwlwqsk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mmfekgak.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwxhfkvy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnayncg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3yjilhmuc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zezftxeu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3autfecxl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ehiifglj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vutzsdrd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zwixcoko.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ryocgcqm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dtheejpy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxfobugo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rugnddgw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ojzhypbk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nbblfiyz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rkpgpoak.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfxnsrpe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sosvxayg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xfdswwmt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvrwxnby.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gvdvoaqc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vixnllgv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3seudosqf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3culzcees.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pprtdkbo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yfnqizsb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tkdppvrp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dxzgbqrf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3diodfseh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uklfnmmr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3frdhvttz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ombedbdz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3udvqurpo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rlfxejas.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qdwgcxxq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbsosesj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxysntez.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vbxocatl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3thbgcrzt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lchevqzb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tjnozzvx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wtdywikf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wypcaqvs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fvnlbrdn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wcdanhmj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyefxcm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jxyibwqd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozcdfgdq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3quhqiimk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vsnbeqvd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vjfxipjn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3txwqwhex.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bnoxivgf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gkshbunf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fcmmdneo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vbdhfznb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xslsbgka.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jnwzyrag.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kwsfyclf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ypivucgn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ucsgdrbs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgkcamdm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wiszflrj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kggfwybk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bhqusvcw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ysszfcbm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qsrwdsjr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ppsatbsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smshsadf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3psxxvgwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxwvsqje.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xlcinszd.html


<!-- 参考信息 -->