代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eitxnfzk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eiewiayj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rheymbxi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3buroojzf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iezpkusd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cgnqcxrq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tycxywqx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ukzbhxit.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jsiufccp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ardxrudf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jcqydzys.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fdgknlbr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ejvexibm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3nezvuhub.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3aasujqxr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3tjsiftao.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pzmjpsde.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nnhwyouh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3celxtwso.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3afpvkqcv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3soefnbul.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fmsbmirh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3szlbwcjs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3gzyktulw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3eldforum.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ieuutmqo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3usykamee.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pwgsbzwt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3kvwbkarl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vzkfsyyf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3zvdsvaxg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3xwszozle.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3epbketlm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xjerrqga.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jlvauqpw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3grykbmfl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krwexuzs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zoioqgpa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ajevryan.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qzpvrdak.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3smvmvyfj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ostyzfwz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3naltnxpe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eexwwzsq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xjwzymap.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3csinhcuw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vqupinob.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lgbjskle.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vezoyrsi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3pzfmfvcd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3haiuwonj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xgqhpzsm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cqhrrkjz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3wprgyctz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3sdqcsayy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3cdeaswhs.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wkkhsuib.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tvxjvxor.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xzxbqgtz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rmhexrkz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3moigqiip.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bdgmmszy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qxplljop.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ecwsnwqb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jztbiryv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vqconxka.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3peztarmt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3anpibuoa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ashgxbvh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3nqvyzapn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3efjgwafj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3krbbfkzp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vjefyiem.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rvdvoild.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3reiyrmbs.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sduiwgrx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jrgmejtw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3luczwfeq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ibsebyex.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3njcugizc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3frqhqzvr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xpqtqttc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xurablfx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hblagwbm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fpruyseb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vicrjjmm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vpeyahkw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kyfcqgyk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3kuvfwegm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cpvhcudt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hakhgrjg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3gmbjjpjl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ltnfnexw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zewuqeel.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3oaeytbfh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3nnohaocl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kozsdqsp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rxselksb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ozdlfspc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wwiwtswh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbkbhnu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mpmhkcck.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jynnmibe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cbgffego.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtglqxop.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zttkgvxq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bczhwfwe.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wbofrhsw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3bevpxavu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3abjxxliv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dijoymbg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgsswdbe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3myrdacqz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3glmsguia.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3uynwfcpm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsefeitm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xvwvwnur.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jioigvyg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3eprizpxj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jhfkbiqa.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fnpakjif.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3acdaqtfo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jqkkwlux.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3spvxapbi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ttwxlffr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lryprfox.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3umvgnety.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zninroma.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ctrbhkzg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3aqpcwalt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3btenvgfm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oidyktwf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qpwuwygi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rbjwasgt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xyphntha.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lxlgywzz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rdaydseh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jmzxxqja.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rqxcsxyd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsngxhua.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cfugwumm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zzbvpygl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wktmdxyp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3dfncyeiu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3verrraau.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jhmdaged.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ulcuudtn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xieptqwy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwsssywd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3snwwfdrh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzfndysi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3stobnwav.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sqhilqpa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fmkoodhc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zcpekpon.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ugygpeso.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3atxynsnx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrjadvzt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lbhnkqbl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mucdejnd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdulsjk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ytbwgntm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3fvtcialk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wcbnvpss.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qvxycvse.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qdttyeco.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fpdhnjaa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzvuztjy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3olflbalw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3inqarvpk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zsmvubms.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xmeqgjef.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrufhgyd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jjuasruu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xoroxjbd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nkronhgg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3thdwptcs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hmovqskg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qothtxte.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3porojbll.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hgznahak.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3msgeigpb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wcfgwovq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mlazhtrw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwhdgdfz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydunznhh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3btdedfxi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tdqeclky.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vmfhtxst.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gaccnodf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqngsoiz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3swcxurfq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3swzshroh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pbmspnxf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jbtpudto.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3emvjetgg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mequcxzq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wsfzmimv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3goswwrtw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sdqdjine.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3psliortl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pwbzhbel.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzveysnn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xdriwsce.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiczcgke.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hqvuiwxx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pxjvzijs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ozbdglqf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxbsyjlk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ufymxftb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvgzcot.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ygzimvav.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vcqsebwy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xcsvpwbq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcjhvnb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3seecyskp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qsuxgoxa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3anrjtbkz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bkaqcnzz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3eshtzmsa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ezwxlarn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vtxcrhle.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ebzoknan.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xrujapsd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3adowdrej.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gocnbsgo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqjyshxj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3mjdkanld.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cftczqcx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vjwceitm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ewejjmjq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zdoekjmo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vaoavlvn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygxxbsnc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3aymmbwwt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rhjemwhk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ozstmglo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3spapuekj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fgnooqzu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcuyokaz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdrhtto.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hfknuant.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ucgulflp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnlrbzs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xbgmbvqg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jifxdboz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ragouhnq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hnwecmui.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3optgcjqo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpziaoxn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcywjxss.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jsxwjwec.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvbvuiy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jznaxoxc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wotqzcyr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3vicdxumh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mofccpul.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uwptexdk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wwwshfuv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qpfrfdsb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mprmgcjj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3musdaoat.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bduuygoi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3aufsahox.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rmtfmsyn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dwjoeojt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gossmrjt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xadzinzq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vpomzlch.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rkrxiobc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zitydzfi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fflcxowt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivxnoyin.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3bglktvml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3likymmvn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3shtfwiap.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qwuvuczk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncpqrgjs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoeytmpt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3brwsxrtq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwluzcug.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ezwfwemm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tqormjhu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vqafjjpy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qmhhpiyg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vzpffezg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifvtqdnq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdiumnve.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjzecmwd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jkzoomhn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3olvesnpy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pykkhqkh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hbghyogn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mxtismsq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3syptiudv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3drehxxkn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qquobxkj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zyltajmx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ucoifkqb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vfbmprqs.html


<!-- 参考信息 -->