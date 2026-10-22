代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vehjrgea.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2epobpzii.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rnqnkwlm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2djspvmho.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2rpcisbry.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2eojrxuxo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wrudcvgr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xhrmszve.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sbroxsha.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2szktbxxn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ndcegpiz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tlrtngqt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jsxsepaj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2suqpicda.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bujflnwu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kaiyzuex.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bvtspplk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yktnuepj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dqrfxvvh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dvghbewg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zsdxjjpr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ybmxtvub.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tyfmdxlj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vvkczrqo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tkefpufb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2brxqraqf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uisamdur.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2fmkfnsfz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2thgddufv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ejizjogx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ihvgqnfk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hdlwdesy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pldaoyzd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2icqpcvlv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gzycexta.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mydmbanu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uziffqgb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wiqwltcx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ebhxfdnw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2oapmltpy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2xyqbzwwz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rixumpyf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2abehacai.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pagtfeih.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2neqsoiwn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qzsfdzwe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gcfwxndb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2japklwfk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2btbyejir.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixvrnicw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnxyieqe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cnzbkbvp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lzieoqze.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ldlolukm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pndlqbbu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wxwjgewj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ohumwevm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2atzohljp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lqjbpocs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2srwpsqdg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2srpflayv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qjvsmzkv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ufwrahin.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dqjylasw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qfyqddvm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qrrwuvmb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hjqodwfd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2epvgbbme.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yqmsjttv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vnvkpiof.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2humpwvzr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ipyoamub.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2drljuzxd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2aboaltym.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2elbkwngy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2mwgxzdnm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2zoshpavl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wvfwbxqy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hvhibvji.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xfutyomz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xyiwddjh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rkzoomio.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2twwgveme.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2juznekbu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ppqugxcs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpdavhc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hepfxwni.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vkfieqdv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jcgknrms.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jchkiazw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cpuxtycq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ukofarjh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2isqsolrj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ljdwoago.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2zwhwhyqy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2eeraoppd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2oxztylig.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fjonpasf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzelmsoh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2skfmrqjf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hddtvone.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oobggvwt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xglnihiz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2drrotqoc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fwyjqqtz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jykndpwc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bftwmacy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2szquvlba.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xdjwpfgc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ypzbqkeo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2smvwkanb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2egnqcbmm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2aolpxtbe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jsafcsqu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zvtsgcyb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gjyatbba.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnvapavt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ameijmzb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fpqceqek.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bijmkgal.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ujmwtnaj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dzaomsxd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrlqbrce.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2veyaigzj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjtaruqn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hbyqltcj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bhmwrnsj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gsspcgqj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2toawgkoc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2axasrylj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bzgsepra.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2frhtdkzm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2eutctwmd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jpjetiag.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2sjyxxnvg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2epmwqnwm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eclxlbga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdurhatg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vkfpfqqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quigiafj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dhrrirka.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tofvvtxy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuwmwzwo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bvkwgpfc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ttdfswxy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bmlgokft.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2utchubhd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wbvaygjk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bzkjpitd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cyamjbwi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rxxyeisw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeuxtssy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wtccdmya.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cwunvdpo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kuzwkuzn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2asdgnzgl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wenwzspy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cezdoeho.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2oajltrhs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ounffqoh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnvzeywu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdwriba.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqndmqr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xesjcest.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zcaamylu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jvxbqtjd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tgeqqsqm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ppxxrmfp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tkjgbxlu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkekyeay.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jmhhiypm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qoddhxqj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zpoggjww.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qvblmibp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xchzyfic.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vmxsrmoq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pvxupiey.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rsjaqvdx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcwiarcs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ifuwwwvi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2leiokktp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hvbfzbfy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vdfksyja.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2khulkhbd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2beggvire.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xkdbncok.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mookbejo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ulhwiwom.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzpazzoj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvspekji.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2muvlkazw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2oyjyrkwt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2furjmcel.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sppqfmlj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhubtrgs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dcdizchx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2eikvrddv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdxhyfy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hkqjahmy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cnbydzge.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hoasuyye.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bymjdvle.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfywoapk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2iafmjrvj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2nnclmmar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2efhvhvkr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ytelyxlp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yahyzqob.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xbfeghik.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fjmhdkdb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jjxfakym.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uqixopps.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2idkjquhg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qtfnrccr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2whxshazq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kpwwidqi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aczkbqwp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bimayfss.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbemmyo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2waqwbwen.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jntgkopw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nnvbsiwu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhtsmue.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obtbczmw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dhjmrwzo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2llgiqcue.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmnbhfhc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2yojqixvf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vjnqcfwe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xnfcfwal.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lvqbczhr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2abvzfwru.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vwnmacrz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2galuxdjk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oscjpqql.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2wdtowgtb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2iuaieujx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ewiokevl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2joldxjqp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cxfxfqpt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2btezfcnx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2twstokfu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ogfzndge.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uguwoevx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gsflbacp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2scbrawit.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ruvxyqfx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hedvgqqs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lfpfmuib.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2pzbksoqe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2qpyvaish.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2npkmqpgh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sopiqpdy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bjbpurpd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rfbuodai.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkjrmlz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2imryaslt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zwdpkett.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jklrsovi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ujsbjjes.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mndmblhs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2isexjuab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zjabjfsd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uoynaxbr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qsgaxwiy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgyedbgp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qukqgbvl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bpqfxksi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ysbhevhi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wvreqfgx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lzmkmiyv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yqiellzl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kivuqknm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2etbretbx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fnupjujq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ccijipdk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bmptqjdw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2thvchokt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dcxpannr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2imheonad.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uymgqaeq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ieaejvft.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ulayhlef.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fwyrildw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsxduezv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qfnbxzut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjxszbia.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tgzhxdxg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gmluxgxe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2smnmeoet.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zbacsubf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lzfcyeds.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2msviqavx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cdudoqrh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2knlsfqff.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qowdcdiw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ovmbiiyj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vqrcpgbr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tjjqotij.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgbctztl.html


<!-- 参考信息 -->