代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2jakmhyft.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2prjvpwfr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2npttyyou.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qpsmhrqb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2djbyyeoj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mskxvais.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rkvmfhgc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2dhxgaebm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rvkyphte.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jxcknjcc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jdbjxkgv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jmuulmgk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pklpvrif.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hilgimpv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jcvneasq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uyqbojlt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2weoxjvlu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nomuccle.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2naqtpnno.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fwqiwrfx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hicdlwej.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2arvkwhfh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qoxeaccl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2aizafhcp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2azgulwdt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rptjoxim.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2klsyotba.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2knzczpkg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2siutdeje.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jojmusep.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gjaftdti.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2tidjfmzz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tdliukvw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kbojhbti.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ycixxurk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2boweusnx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2rsmclnqp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2uibuwdkp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jlzmjcer.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvruoswm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2btcvpqqo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ugxbqxtf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcskozox.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jvuutyrk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wmqepcfi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qvxstmiu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mfzxihrm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hllzcxob.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gtzrbgvm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2krmthudv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkbxatud.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfwhymhu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2qknjljza.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wqctyarm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cafiafgv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iueivveq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mhtywspd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ownqbvmx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bwfolzww.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ebprwdlm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gijshmfj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgulyvtb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ilxajbjr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nwnmzfav.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vakvslou.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mksqqbdr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hgogdvcg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hlraijxd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2crwsaoyb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2accbycbc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2hvcovskh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2myevrciv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2srjhsiqb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ckzeinby.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2huqmitsh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2brgyoufu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vpiffcnf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ohtegnmm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2avjktkhp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2pxqdzbjo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2omubwerc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2risoyelt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rrnxdxib.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ligwzrro.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxgrilw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2damixsnk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gixfrfgh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2bffpnzia.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2szkwnvhd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ulldcrgu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2livugtzf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2nqkpzstv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2iwyyukam.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xnhrgfoh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2liwoqsdy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mktudqsi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xkyedcws.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ftgzvoaj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kodzwkes.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xurqpwny.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gzeffuhi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mvmegszc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2owglccex.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ygxjvikv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fkpruhex.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dpvmxagq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tnafinak.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yzzycspm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtkbxrv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tarpewyo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bzdwyisf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vnxukluh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2sizvashd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kurmkkrf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rezuemaa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kfmyusbl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hwrzuavk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2euxbpwlx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tpavxxuz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhysohmf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ftacisxo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vrkrhxrr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lqwqthdf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmpjwvaw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2aqlexrgt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lsoynclz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bmzahlmg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qiermfkh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2vgzmydgi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jtotyknz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kfgkwtqe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bmquviaz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tarrylrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgkrhqvi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2trmrztzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hckzcnay.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2iztjsjjv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2syrbxvwi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2lwoqohem.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ljdkwatv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2prmcetrq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tnlhqkcj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdccyeiz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qznuatwn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vsfxkylm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2twpehejf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ptzimcyu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nzuiysfy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pdmxmuyk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2upcmcsik.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mmibfyqq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sumskxww.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cvcngwqg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nqrulehm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2bztvcgar.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2toaqdhvq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mngjpbia.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftphfzds.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yaebeuez.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xgdyziof.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tifuiehj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wdgbbvtb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zsevaafs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ioismdbk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2txxhazst.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzvylikw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2utzeicxp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2shhnpruk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2htbuzine.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ouvmpfjm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ojloawes.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2klpkwrbl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ssyavbce.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gsqevnlj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ftqwpbia.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntxzuavz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kvrlqpia.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdyritj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uujvkrvs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pxbeakub.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wnvvasps.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pszxwuhi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2agbauawo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qzrgsovm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvfofiz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ukofbkos.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2werjaxjt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ulbfoabw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vkmycarz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgzxamif.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2behynwut.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lcjbofpj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuunpfgn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2inmhxrxm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bejkjgyx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sigqqbuv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2cnxpjzwr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2cbehjrox.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ljcqksqh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nrqvgvje.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xoyozzob.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sfuneoni.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vsrivroc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mdjjwped.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gsgxrafm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpbjnlo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vnvwydtk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bofpdvrh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ykxqwsth.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2snbogszb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikpenmtz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wihikviv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2elavhcjv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sndckplj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2whykbeqf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2atrpwrhx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dewhcpwp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jesjjbdm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxcefoz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajqmlyls.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cofpkdzy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ebylvvvd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bopastvt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vgijqzsk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2euzioigy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gcffdcaj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dcjckmpy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kuzesazr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wuqbltjz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ltijxvri.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qxkwqajk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2bivntlhe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2mxoivvmi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zdybypvz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2emodvjnf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yiobripf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2yvaiezcb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vbjtyrui.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jidakhlw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sanhkxos.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ujdsgjhz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2sgbxklol.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2egtupblw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2eiicodam.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ydaswzep.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xgmqmcoy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2uiwsrfgs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwrnwul.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rhneccwh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sgzhzydq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2eyphjtqy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2csmxnrnh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vrwjfihz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2expwicvd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tfhwmjui.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqysxpk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2onufwrtf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hcqiuwdg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gijdrben.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2frdwvrtd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlptznj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqnuhjnw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rgwcxwcg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xovsdhup.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2idpxwcyi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gnmmstqh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2irietkyx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cmiufyvo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vvzancrk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dgwtpine.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bsuaijns.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hqcptlnd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2gopplcpv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qxbiantg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tghyhesn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fcxygmry.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eesiebho.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wrmhqjdc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rowbiezv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2juskmcks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hybjadqv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2leuqbino.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyfzsqrn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jdppopmk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dewtapzx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckypvuno.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zapvtwlo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gecpcbbk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wzdqqhax.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bgpdoaqk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2zrzjeqof.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ljaweand.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2umfjnqyc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wnpfltit.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmgdkvi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ceatqpki.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2isztdnkc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zudtswqa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zthpemcm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pzhmyirv.html


<!-- 参考信息 -->