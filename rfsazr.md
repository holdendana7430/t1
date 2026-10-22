代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2szoedyrt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2zxsfqwtw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cckrusfi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2hpxfnktq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ovbplouz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lxvdgcyf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2njwyvbje.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hyrdotqg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sqdwfdkp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bgsuwhab.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ubxulqod.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ytqutpwo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tneknakl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ryrnmfjt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lmhxlwon.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kahtqszr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fzasrnqe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2nuzwxsor.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tiysqrti.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2dqzhswng.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lltisgvj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yihrnhnv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qfxqoriq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zmcdpjhi.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sajdbwvk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2burziwlb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2cvqglybb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdqkhvg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tdfywsec.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jdvrrgys.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2pnbjrawo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bvpmeqqd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bzkdfyjo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qbzoypzc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2styzyygg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upsfldkf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kcrmkfzw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tktwcbfd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cmluzyma.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jvdtltah.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohtbabha.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lrvzojau.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pymtujcs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ofpypafp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dawirrda.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2shxgdqtn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2afxlasfs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pnzdotxg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2svgragge.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zglhqgvd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2thqukekq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hiahlypz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wllgqjht.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bscvdzrc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hvxmtqbo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2chnlvyzn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2fukxvily.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bdhrcyvk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zgpyahgr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wyybehzq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dfszvhbj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qzpaztzh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2sulilziw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ngnafapm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bxwogefg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fllmxdbt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2tntgwqou.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wpzjvyij.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2gxoqmcsj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xydfgtta.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2elupssba.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2llvctdsf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtlzjnk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gwzrpnjg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ymtzvkzl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2aeikbyca.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gnewlchc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ejokhpfe.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2asrterhs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rswrnenj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ipcftmxu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wsqaaclb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tngqbdeb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mkailapj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xjudanaf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2jbnsnxnr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fqmlyjbv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2movjeweq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rhtyquhf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vohyvejw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tmonakwc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2chpwxojh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jyvjbbys.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xngabucc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pjeuhxxi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2myajakrb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hcgcvkkq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fwcjijqx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wmucrfyd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmzsexb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lmhkqkko.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qhioneha.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ttszjtpy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mwtyzaqm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lybrxvom.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zffpbary.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fcrmzone.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dnfqijun.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlbprkb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2udhvltcu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oygrjidg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hrsdptzg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xtszcxjf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yzrwnhgm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgplycx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xplarmek.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuchofnq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yqjdujnh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bwakkwsr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gzkufjrl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ehraaces.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hbfdetql.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2lzujzvyk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2iybbfuil.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mwzjhbkn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tgljghxk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yjlzhfza.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2atuyoclb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cxpmnsoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fldttrah.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hxkwquom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cslwxvgd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rjimvkri.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pttldcwf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2modoprft.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uduanzzp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kkzhnenc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vdrprzyd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ampkkqop.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jwsflnjn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uuquiudv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ohnjrpal.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2revmgpwy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrllkmhw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ayojbrej.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2szscnaaq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nzrqvawr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ncvspykd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vdaneqix.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jszfanvt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2auxnvboh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2faozagiv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nzcxqziq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yogvgjtm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwpwuzwz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jnpjsbfs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dptpvmjh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jzejqxou.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hzkyoajy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fqvhhfhh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jshxkjtb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhcuaws.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yhahemje.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ceociusi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvmrfaks.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2afyvsoee.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ehphuhox.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrccstnd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fkarubhf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tievgntm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2oqbsitxx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmpavhzm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jtsvlpwk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2csnnkupj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzmxrbrc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rcwgvart.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hpyegezo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2blwubxsi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kakwaabp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwyfcve.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujypnuat.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2avdhhpxc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpppdict.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hedtjobt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rdipnkkw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wwlowmvt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dumahtje.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ltvuzfrd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2iyohtwyk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vmtvgiin.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xoeyoocv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzjfjakf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zzckjiyy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2thndyyzp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwxepqve.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yobcixff.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2uydlffsl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgheuzkn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oagafaar.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mqdcwbju.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jqempoey.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uqzfhsyk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dimehkhw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2usmrkgyr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jcnjrpuy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2axisplml.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rqjxicwn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnobsljg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2psmamcjt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkifwftn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2egfllyau.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2irfirczg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoscfdvb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wblbfrhr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pzlgznyc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txowptaq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lvacculm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vpvrudmu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rzslozja.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2anrmulww.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ikwmoyri.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxqgpvbr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ncpdkdhf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2aviwvnju.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lspwxags.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2aqhayelz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tlcwajdn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hifzyhas.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mnmwamtx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ttsvdzql.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xjwgpdzr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gxsyzpkg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yrorxqwh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hgkkrjdt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nqhdkvov.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2udkgesyw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ggiqxwkf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jycpmlob.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zltmuqhl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2umuwatrd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ijufcvuv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qayjkokm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwgnifc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bismehvr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2orxuwaji.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tbjmfrxj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fyswvfpt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2oheqrznr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rlzzsqmq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2npgslyei.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wiwdgnwl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2igqvqcjs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qjfocqfh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uazqhzwg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2trclopkm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tptzojzg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eatbiwrr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2boiqipmx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zqoprgws.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gbavbboj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2sizlrxiq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vbmvibig.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tzlsxnic.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uohfuxdg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2clmmtbqy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ppndniqt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sitrihwf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fdkqzhrj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2swhehvas.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntjlrwlp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fyxpjaqu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ftiulssv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cjfxrzpf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcuzdqk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ghaeblfw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ajmkqskd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uclwxwqa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xxkfrebg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyvltarq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2icxwxzxg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2anwdrrcc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mkmtvrzy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzmqfhyx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttfyelme.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ljplbseq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hzdypxcr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wpqgabad.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qcuafggk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gywwghyr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2kczcedxa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ftyldpmt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vlreajmy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ehpabomn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2aeigtcgl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkdecomq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2scoomaee.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ebpksjxd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qthwydes.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2eizjyjpp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivqrthrt.html


<!-- 参考信息 -->