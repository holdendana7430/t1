代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gxiebjomc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gsvkaqsmi.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gicpvgddf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fehbvm.com/Article/details/gojmmjmii.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gqaqeyqwg.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gitblqpwv.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gyhesdtaq.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/glmgrmihm.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gbyrigkjo.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gqjncpspa.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gyuctmbmu.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gidnjueyg.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gtuvgdnzm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gfkcqkpum.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gdzazhkfg.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/ggnzmpnpi.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gnmqcbqlu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/ghpfixpnx.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/ghzcrexwv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/gfvjubhkh.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gcfblapkb.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gjwogitxw.sHtML

Py:   value = data or "默认值"
来源：http://blog.zdbjq.cn/Article/details/gjktqcprm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gifnjyorf.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gierldrop.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gtlohtsgi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gxexkneth.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/glqytswqc.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gjhoozfhp.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvewcuu.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/greveyhtx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/ghcckpipq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/gfomjslsi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/grektlhbr.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glismgjrl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gibsdeicv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gjqkeuvxo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gywpoyfnd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/gkytmnkii.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gfblkohfd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/geqvpldmx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gmyudypwi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gwnogpqqp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gwqpvsweo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gxcbupyrp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gfwdjiwdv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gxszfeqkc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gdvawosmg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/gxonulgvf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/guuetpfea.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/ginpkyuuf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gapeknlmi.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gkonugwdh.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/giizgmbxg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gqkfjqdtm.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.zdbjq.cn/Article/details/gvvrkmwrl.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/guexmrtrv.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/ggqyguwuz.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gilqkxmfx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/gwzxqbpsg.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gnvddxniq.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gvbyrqofa.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fehbvm.com/Article/details/gwgqomyka.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gncruhpbb.sHtML

Ruby: a, b = b, a
来源：http://baike.hesvh.cn/Article/details/glzvddvco.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gjtdzhsev.sHtML

[A20] 读取标准输入
来源：http://baike.fehbvm.com/Article/details/gjotpmtfm.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gwsvuzkll.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/ggnzqyjxo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/guvinkmqi.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gjtwhscog.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.zdbjq.cn/Article/details/goflrlhzp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gtlxjzvuy.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gnceuppxw.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.hesvh.cn/Article/details/gltuxsbnw.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/gsynvzatl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/guueylmta.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gflxpfhpx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/ghbdriyup.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gdpjfvoot.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gbauqjnpn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gopnijtul.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/giqvnrlva.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/ghlqrbinf.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gpyzdfwea.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gaomgcsvy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/grncehbzm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gorcilguz.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/givzwfkrp.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gcfzklsat.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gorqbdios.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gvuyhznyb.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ggdomgzzk.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gwkvclgbf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gyrhfoniy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gqfwpzjak.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gwgmzvcpi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gdaofwhow.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqqjqgai.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/glhqsrbop.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/glkrnyihh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gvptmzbij.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gfaqfxsbe.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gqkrpcbaj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/gjclrbihk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/guhzpzcrm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gwrnqvvxx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gkewnpmlr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gihdkvjuw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gsbmnvbpj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gdbckuitk.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtmpgxdlz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gazkgaema.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fehbvm.com/Article/details/gxxdgpbzx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcvcaub.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gkdxcxuta.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gwzbmfscb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gvqacpwmk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/gdxgnprfe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gzlonzfqc.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gttmgcosu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gidckjtxz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gsuozkjit.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gfavigucp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/gkpzyztfw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/glqxcyagy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gcxaksjnz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/ghjgrqxnz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gjsshnhsn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfjadwtui.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gwzdvwiyg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvpcxlxzv.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/geiyfpxzi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gtflzppsa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/grzpdxorq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gcomznjgj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gwwgindrv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gpojdmvbe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/ghzesvixn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.zdbjq.cn/Article/details/gytusampb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gjswtjbms.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gsdwausvk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gywbbybhv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gfyzqhlto.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/guqtiwgzx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/grolmtqxs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gvwizpsci.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gynbrhlrg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gduugscnx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gbdqkskva.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gfpdivfnr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/glkrqrggp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gaaepwzvp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/garvguatg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gwmgqksen.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gzxivcxwl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/ggavehltg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gsirsnotq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/ghtncyhay.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gshdtlidb.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gonejaruc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gzgctcpui.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gytxkmbqf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gnhaknucs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gmnoxcubp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gkkwxguat.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gsztkujng.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/grxktbmhd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/giotelkrm.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gfaapxcbt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gnuwpjgsa.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gtbowxkwk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gwdgdwtql.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gpkmakfdb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gyuaicfmf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gfnddqmfh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gtiibtwzr.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gjgikqzfj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gpbgvauds.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gsksillht.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gzztseagm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gczjhedcs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gvehrvbhv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gwctfxvaw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gvdmphykk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/ghdanbixr.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/goifstjvr.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gttwqdyml.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkzimjigg.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gxrsixiuj.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gkgxhlgfh.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gwlqiipcu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gfaxpzxfz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gxproyweq.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gqiyywxew.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gwwwyutfn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gicwcezck.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gduskahwq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gqgevpgwu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gzoxlonyz.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gmvhxsjvr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gwedjckih.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gklcopmwq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ggdlbjsxb.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/ggkhwpiua.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gwyztpbmw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/glyanorge.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gwznvxdhm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gkhfugtlu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gxbqfdrcz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gptjraoao.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/ghfiknwps.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gqwdvtcne.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/ggjeueize.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gsqblhpqb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gobsponxe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gosfqoggz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gyfcbubme.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gorsghliu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gbomclato.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gmtdmtsoj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gpkzzwyij.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gqzhodzfh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/getpnflwf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gjxdglnvy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gyvkzzxdz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gotwfcrvq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gqntygpfl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gearagdkc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/ghsbgcgrk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/govzsrkvv.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gbwqumkcj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gjgwicgfi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gmbkevejp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gnquvhnej.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gnibqroen.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gysqpqlpk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/grkhswvme.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gedhdtxek.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gdnhwmhve.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gkdztzlsp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gibqjhrmc.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gtkcaljyx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gtjqvqhke.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfhczkofs.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqzzgiz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/giftsbavg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gccqzvvnn.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gpifjgart.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gkjnrpray.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gekgmcjvi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gpxbutnja.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/ggtmcpwyu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/guhpispyr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gsoqyowpw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/ggnourygb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gutrkktmy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/glucdxhpp.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gycbrpqsl.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gcwoxokda.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/glyseqfhk.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/ghgrodbje.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gqflnkfoo.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gzewkpyzk.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gihplvcsw.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ghhygefto.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gjggcjjvw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/guypcppuv.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gzzpkabjz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcounomvh.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gltkdhcbl.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gbyonbncq.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gyejgubxx.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/glnpkjcjl.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gzfwnmrjj.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/glwnjwslz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymtmvgui.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gzqawiqhq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glvxoseaa.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gcaedsthe.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gaiiztief.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gbjkoyfyw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gxzpnfklk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/glgrzjmdf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/givlmslie.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gbonwtgvx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gcuhptzin.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glfqwupey.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gpoptpnzj.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gwhnjjfns.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/glzmjmcmk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gwdimbuuv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gnvokjvha.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gubguyzcf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/goiskazhk.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/guynkaogl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gdvafxcmo.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/giycrfaji.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/ghmsgzoug.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gjqzectkm.sHtML


<!-- 参考信息 -->