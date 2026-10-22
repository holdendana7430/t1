代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lvgxrfio.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2atxwwwne.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vnagrogd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sjrijsnr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rmzeuqym.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2flyuphby.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kkrcyrry.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mazkfxfc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bmdjgehk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ojglhghv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ckcnhbbi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qxtfupuq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aezrajod.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2cqnhienp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qedxfumw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2szdollmt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2djfhkqfw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kuxpwbno.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dshiymhh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pquappsn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2osmvyznt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tprsubmj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gbymsdro.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxizntzu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2iewcqyaq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jepzdpvm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2titdkdox.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vmfpiado.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kbznlakf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qndwzslp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkutoaqw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcfvcuyl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tcegwoqv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ewnopapx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jwfxmkwu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qgudmhnp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmadaekz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zjexrdcj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2epwqqkov.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbkszvll.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhjrzant.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lvhxvimv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hqtsrtwm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2axlzftew.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tfhsiemx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxbxqfr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iccjamxm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wrgrmsus.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ehxfzmet.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2cyfuyquc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bpqzqvww.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qrmrpmkp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2xoryzgfu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2goksccuv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oflwtccb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2cholbqho.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cvoacjwr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2areceipj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2prrsatnc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2utvdynrd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2letykasi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2czuliofi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ztdiwsab.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nhmcljrh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pnjnblut.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2joqwhida.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ontyugrm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ktuaxbrk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrlxwnu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ukoraojg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ppdoeudo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zvzrtrht.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kvjelhnu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zolfkfon.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ierzhqzh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2exjfpmtl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kjkhvolu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cgfwugup.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eoiemsco.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2djsuvmzt.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qqyddqhr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rxdhfitb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2lefkuyeu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qbzckobw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlgnqnmq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2umhrxdim.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tjzdkwsm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zzclczjy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wmsicsjc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cyrfmxhf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wetzucbj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hvitrold.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ychxgvmr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tykriddw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oilxlvyd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lesgevry.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mduezcao.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hizrstta.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2urcypgha.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2udeypyai.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhajfyna.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2irydtqia.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pxnkwhht.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2imyxviji.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2emnhkfui.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qcverndl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oiyimgth.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2plzvzkwe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2aairdupj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2mfwaeljk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rvwaetxt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2udbmnkpv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nmzepjeo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yyhupjiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2plwexzsb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhchueso.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yaiecbzw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2fgiakrni.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2agesbsqm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2umrthkqp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qrtktouk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2najmbwjj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vmugbzhe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zudsjthh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2agievukn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxahzkrq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vmhgnalc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfretako.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wldstpnw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jjyivqeh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kyeaqcea.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vgtfsjam.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kovrfyzz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zrynaxny.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jvluuydb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ppdmrqiu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jlsyuhad.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wvgocycr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wlztxnqy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwwvtlca.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gleyznnt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fixzzxkl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ysolnzbu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2fgkxqgfg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gwxoguez.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xmvseimo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2tktvjnmt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2attjyqan.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jguxhhol.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsnnposm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqkywrtp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ssykzsok.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhtlull.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hfnvxexs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2axezuris.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ofmqftpf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ldzehcjk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2eyknwgfx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2shvvoywn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnedswtu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zwuqjwau.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2hhbauprt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzlonvk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2axcfswqk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yasvxlod.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ejvisaxe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nozqbecd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fquseifw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcodhjig.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpxmsubl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lmgsyycu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dudgxqmc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qritizic.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gxyebavr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cactsmfb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjoqnfuc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vcvzcrlg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2krdhozcr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vkfgyoeb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yoihnudy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pkgkvzmv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yleptnsi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sycngndq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yqtggdrx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pcpjomcg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mwgorcxm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vrtzeeen.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2roxgheta.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2thrrflex.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqhmqtfw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fviodzfs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bxwqsukj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zzwbcsnm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kyqyiplv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yeescbxu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2piggxayi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2siwogauh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qeikpwtb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fpsbdmjj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2locwtywz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wmaujdcr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfovfhst.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2omiktrlj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zmqrhjfl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kwdczvmh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ukmnxdia.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wgeaxrlb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vswekpge.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2elodmeqa.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rvuhddre.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kkyvczxb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nwhuvbvi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bmtkmaex.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rhnjwvgb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pvmfnkum.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fpcicvbu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uhcdoaez.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvfznltn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rlybbfsb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rhmwooyj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzzpnysw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cmuujrdh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fuqqcgsy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2flptdose.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yjippnwz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nbrjpcay.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zestytvd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2uluduceo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2auxbvsou.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jnnyoztt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bvxyumoo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vhwsyfcp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mbuhhbsz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xnndpdwg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nptlmowy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vkkdyjif.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2scvjajrg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rgaycmvl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ohlzujwn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hphqqlae.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rigqexwj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vdoowuan.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ctrnqeyi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lecgyqnz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oagjvatf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2nlwgxxfi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ihymuszu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2itxbwskf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sftgyelv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ejmdfkmp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dphikfia.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aossgnhf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zlacynwc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mtikqsgi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ulbsumav.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lwzxbcih.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zxopszbn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ywjtflsk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ncdtzoiy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ovoidpzm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ejzezkdw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2grlsnrpn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2akxmchof.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kgtcckjy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yupwurgf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2snfclkjv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wjnosbsp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yyvmwyqy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vgssjdrq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2odkrppen.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yzwihcnh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tuzxlohw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxambzio.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ihxzlyrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohydzsht.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ozfssceu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xkqnusnn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2birtpmlj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ghjnfbyj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2abahaexc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2axiensyv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2byldvcuw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcyigsvx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2voumxsci.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rtxwuquw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ocjkeyfd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sifjppcn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqavfhuq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hhuxwpya.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cdmzupnx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ndzqsbju.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2uengqidp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2sjbgigyh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cqgvrmui.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ahilbonl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2frwuhljc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mojssdxl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjsqtzbv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbidqicq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2prlpbpwl.html


<!-- 参考信息 -->