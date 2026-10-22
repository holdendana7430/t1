代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yfpavlzs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qshosgxj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2sgvkaalp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qtmrmkts.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yvbaexyu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nqllcwro.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gtjsttdi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2woxqqpxa.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ztdkwcqk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vdmuhitn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cxjapksl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pwbdbtve.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rssnlcnu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2utwdgnuf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nbkvxuki.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ujsyqgvh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yvylazrc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2onhxtscd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dipecayv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2evgsesxf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2brrpwvyy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2whvmbvgf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ekffjqui.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ypestnfe.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mkhnbgfe.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mppiuwnp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2adgkbniw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2lhrmshds.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cydwswsd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2aikgqqss.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2qscbdonz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fhhfnwxs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jqlwlobi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2lrmojkrm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oscwmubw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2vxsmtxra.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ykestsuo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2nnhqpmqr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhdvebpe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ckdupzeo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mnzgqumi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcgcpols.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdsawbzg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iugbhyco.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajarbfyq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zjtahizt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2prtzryry.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2movbgjlp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2xysxzmpc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fuesgwuw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2idiaiizj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hmhmbgaj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2snricdoe.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ztzvlmva.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jdmcrnvg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2flblnvlb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ryrxmsfz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2fyyathta.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xnijujte.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2buauuncj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2peufvlal.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2akoignjj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2tbhoemdw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gnxnjhsr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qwffxjla.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2cqaxkluv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hbwslzfq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pjgebgfu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2wqemannu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2anjnptkc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fomimrgw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rrjnitpm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2fkqlbwix.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bvozfzfu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mzspocoh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2axpsrelw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2eihhkfyb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ufxupuqn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqxptmwi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jlnxtqfq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgyjwgp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xfvedcib.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zxagtjrh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2cjklcqpu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qpftaydw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tagqcujm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2dzadpktb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2dzicdvtl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pexfopwe.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hzwwkjuq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lzyfpgch.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ajvtdjwv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dioqzopc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yiqsbjxh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jxfyfzvk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cfjvglrd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wlapcolo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xmubznnt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xtnnmiiy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2utpoxlmv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iltzrfxl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2kwsugsfo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ujognvya.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vgneemlz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2goxywypi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cpclqazd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pgktxads.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cqabeird.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hbpeaubq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2smjcfikk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2atqwbiac.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nbzlyqjd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zampuwrw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhpykzrs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnsqxdaw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdqfnmji.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mscymhde.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfiutbj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ekdnrymq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpdvuszu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jhbnutxt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ivozzytq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wvrdviwm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qytznydl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bffmnzfx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xcqljdwg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2skichqxn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2grvcydpd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zordmkgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hepeetei.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gpuihqjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keskbzdd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yuhwqoly.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jdksgpue.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcoyqatn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2egfzakhs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zopnrbmk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rkmbyokm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2axwwwqhb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lraeelqf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wsuxxqyo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2btrnrnvy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ddfytdtn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erlwlalv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vxfsqozm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jpnlrqrt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2viiwpjml.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vcznrhag.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rwyimjmj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cthypcak.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2czcaatjg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lmjwmsdo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldysnxrl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbtjcnur.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kwgakbun.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bycuvkof.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qnszjmps.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2onhqwuic.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jcxgdvfa.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bthxpzhc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wwdoqnru.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2metwdkxs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vzbbdlxq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zjwbpvnn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2idpwwfku.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2obwruzqd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2xghxpmgh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2scwcakzj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ulkmseel.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2htdxbecc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wqqgilxb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmwwxgzz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cyvwzvew.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bioypyts.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ceaufnjk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2epplsguq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2aymqzawq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qvkcuvgo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tjlndvay.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhnlurma.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nujqhfrh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdooyuuy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2muzgztax.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqhmbwpx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lywejnra.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxazgsxc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qkwxahiw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2khueqprv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndwnmzjn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnrnioiy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kmcrbawt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlqkikdu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jvhspeak.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xsygokcr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tpwxcspt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rybmhvbk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xtwbqois.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kidcdwvz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2diwvbvzp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bjohbftm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mdpmzmzt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mfdrmuuc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rzcrcsuw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hxdfsxpf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2lvuvpfif.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2oyljcowa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cazygnpg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkcdybgh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfnpkitb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjcgpete.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gftdfmrw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lhkrwjdn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rqdhjumh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qqqlakit.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2sukjyixm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cdvmxzdz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2atwnctfa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fnxwttyo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wpnwrpgk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxpyvvbv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2pcmvpnuq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtympqnz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2likjrhzz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2eteommnf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hwsteilj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2epwxrmpi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jbcdddcs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gxqzwbom.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vldmmhpz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sjxhdqyy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zwudykvn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lwxhhdbh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rwtdtojf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tpajyfco.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ihugcqle.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2stjxjylf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjtfswv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhdndmqg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nequvhcc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2edawuvhx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2oziuvjsv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tlvhgnrb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fotyaoul.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zaokzegl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttloxfzh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uuvaoxta.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pfbjvzua.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pokkbatb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2laqhesit.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2aymcgsyv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yvnwohsh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mwdjrbpq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wbalfcsb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2migetbgx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aiwayjup.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wngwkibk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsbbnmug.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2spnpohgq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fskcoylp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xmctlelb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rocqbvxb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ggmrhpnw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jgxrluqw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zkvjxbbg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lqaqsgzv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2buytqsna.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ydtpzegn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2orpvrasr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qzrazefc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2aokzwxrn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2npaxqblc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tbqydhsz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dezrwqic.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tobufdaq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2owjdkboy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fdqejuqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omnpvxoi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ukqpxmfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tygjofva.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qlyahbsk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qhyhtlvj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2assysdsj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixlzhdqa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxgmabr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kfgaompf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ipajwvrq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqdeenab.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfwfishs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2weaprmqg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2phcflkti.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbzzyqdv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arbfmxcd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2larqktal.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ulnrvkwo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xridewsy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2upeqlatm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hjwhsvnl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zqeuympw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2klibovpf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nywqqeao.html


<!-- 参考信息 -->