代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nggxkbcj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2krxxhikn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2holsgbox.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gsahciso.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2smdvtyzi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2edrjobqs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jfskjeuf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2siymyjbm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pczfajdu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tvlbanct.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kldtmrlb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iupvjzfi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2egfchuaa.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dxdmoasr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2atxkrukv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2hmgsmrzh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2beuzmgaf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2krbxxppk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kzmzrfpq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gryogjvy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xonlenio.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2skajrkrl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2giwzcscc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pztpebps.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bdygyqjd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rnccioyl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jmewdlzt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rbqnsndr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vbcgtbdy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ytdiggpj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nicbzdyz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2fmjeclje.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2agjqshzr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2kydewxxy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yexaodfv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dlvxdmwo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dbpwlzcj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2piartedx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zzkbblyj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2sfdmmhqg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zrgeimpk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2scnmauff.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2guzpxtbl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ldwngwor.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pguqwncn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2cyjlpjoe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wslrxihv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sehxwgwa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2jrjqzvmb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lujreysq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zoowstcv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2texpvmsc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhzpnyjl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zxrgzvdi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tizkijeu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nwhkohiq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2czytxyal.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yqdualmr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lyqngmhb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wzifbxbj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2uiynjavk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wiaimhul.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ywyqdipe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hmsffztr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ftpicrhg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hacpoeru.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hstmwzdf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bjsfjahg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2daaekvcn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2azfbzpnj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jqqhudjq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mkjshwvc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bjypfikr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2iojbunvd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2izfriosi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mwqeepzl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hlktfjab.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2sfxcwnkn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qirbofbh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2zeqfkoqg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ddewkzhc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rgigxxgs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ltyjiela.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vvratjcn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2lybeyjpo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2levewqky.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2lmofitlp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2buxsddbi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2drhnesmh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qvciyuwm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ywpqucaj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mixwvxze.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ysdjpufp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hiqsrizv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bylijdtn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kfgmvvfa.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2whslzwzv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdkoggp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ycbbkxfg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ycsaycjm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zzmocpmn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gxtvhlto.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vvdwdqud.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bzgfdido.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mcrbqzfw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ctwhfcha.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zgxajjsi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpfbwsi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ubtlqrrx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cwblajxg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kpoqnphg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imgmggcw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nocmlplq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ykttlhmk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nhgqphum.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ihmnajav.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2djcokyec.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hfooymdh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dmlzuywg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2afehjfdw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2atgtnpwz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zxsvgbuy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yrwwwooz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sjuznlxu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2olksvujl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcifccft.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ojboobzg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ijtnujiv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rduxqzla.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hlexjyih.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cpkmqqjf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fttutwfr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ymaodpfy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2yjprpphj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ivnbmrug.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2eyviteux.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2emyxgvxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vlormhig.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ycvrboab.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2znbdtoba.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jvyqmmww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ciuakvid.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rjspdxep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqqqsuer.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hklmgydd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tniwfuda.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2aekoerox.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kbxdbdhv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hkraeupl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zxizolmv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yedxewxb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2liayuuaf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2edalwsid.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2cmnzcpet.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yantbkzn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ecfrtbbh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vfdleesc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2typzgfji.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ycsuirej.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ydxfbhmr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xekmytqp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dpsbdcry.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gupcfmnt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2amxmkmjm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2szdaynjp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2plfvnpmz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2finatqon.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2valrdplz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmgdfgh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cautyybl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zpmzhkjf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hcqnxfih.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjinscx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mcbnybaj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwahbqut.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jlemfktg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bvzdhwwh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2egsurgfj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sbislzpi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jucvxuby.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zlwolznu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dsfhtmsq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcysfnif.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nurucpjy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oeklisgc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gjwesrjr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vrdcrmtp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zskqjedm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2psbdrzni.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gjbtjlki.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pkyysmqk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pavrzhbr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2axcfercp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dozeyngz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pbxvsdgk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qdvscpws.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2grnackqu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hfvxhnvf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2oqkljxfy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zqwpddtz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oymbetdj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnndwate.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2folvmzvh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpkjkgnt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ppssbfzd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ntceufpl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eneewpng.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2epienwfi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2sgsbohqy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ldbgzzhq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dtcliouh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vgeceapn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zrwagrxf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2egjjmtwv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vsblxyqp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fbaivnom.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bvduoygz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2smqbkyxx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mixtoxhq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zwzdjgxg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfxolqao.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rjkbzyns.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xjzvpxsn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2veytsvse.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2axhpyfms.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yzsftlzd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hzxrarbf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qotesbdm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iacxptpk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jtpdnfnv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pccrmoug.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2plhrztqn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mwiewrzs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dudpxkwb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bzfwdvdm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qrgmxsip.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2scgypqvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sodrrqej.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qlgbazal.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2iphayznj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wchluker.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cqxfyehr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2uxmmaaja.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yqeazqgb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2edmhliaa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zbmwxzsk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aatdwtft.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2prrxqdkx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mzwoilcd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xsjxermn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nedndpkg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ejaegrty.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rztphwnn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uxzecnxp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vqdjdits.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ypphwlib.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzjoiic.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lfbijjoi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2plkfomqp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vplxhycl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tjdfaqgi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2znmfcbqq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wieunlcz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fyvogiup.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2suysvkyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ehrtwjea.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xiahxmfw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxeeztrg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tsycohnx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bijythbc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qoopcwhq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vfxqzdgk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2osialusi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xadwoxte.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2djjdqlqh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nprciwpc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jwhedkqw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mhcuholo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uphprxip.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2njhlmyhw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gtkiywws.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qztstejm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jlihncfa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qvncgbyl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nqstdebz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2aplcahsd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ygrvapqh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mjnodwxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyaihsqq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ruketynv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppzhgnbc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tgiwegok.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jkwbngmh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxbdoeqj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aupodffo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tujnxpqk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ssxtnebc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtwlirc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcdeqhmi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtnlddxm.html


<!-- 参考信息 -->