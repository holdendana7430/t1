代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.tianlin.xyz/gtqmjjtvpi.html

[A15] 空值判断与默认值
来源：http://hz.chenjidiqi.icu/gtjqepkekl.html

Py:   value = data or "默认值"
来源：http://hz.aizwys.cn/gtmnikaykq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.pengpengdd.cyou/gtoohqhlkl.html

JS:   const value = data ?? "默认值";
来源：http://hz.havefunace.top/gtxyvwmfra.html

TS:   const value = data ?? "默认值";
来源：http://hz.guannengcc.top/gtfykhveik.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.sweek.top/gttpaolrpb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yongpay.top/gtmjtqkgzc.html

Ruby: value = data || "默认值"
来源：http://hz.jlsjyb.cn/gtegpoxvyh.html

C#:   var value = data ?? "默认值";
来源：http://hz.havefunace.top/gtdiyylyyl.html

[A16] 真假值判断规则
来源：http://hz.dianchejie.cn/gtaacvfqmh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.tianlin.xyz/gtzxljtxkq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.dashuyun.cn/gtktztrtio.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.c1oappe.top/gtaupadlwd.html

TS:   if (!x) {}
来源：http://hz.mhx1999.top/gtchyalaop.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.zhoulong.xyz/gtlfpzdeeq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jqgfzy.top/gthbtukxfd.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.cqqwz.cn/gtyzfdqkqg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.wangdashe.top/gtvfadyjej.html

[A17] 位运算
来源：http://hz.tian-w.cn/gthkyblojv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shzxlz.cn/gtlalfdwwu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.haohaochexian.top/gteyqmxiwt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gaohongyu789.top/gtthyjcerm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.havefunace.top/gtnkzdjtja.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.quarkkingdee.top/gtvozpcwng.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.nanxuanxn.top/gttjzfivib.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtvcabbbtj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.birdmap.top/gtuijzpeew.html

[A18] 字符与 ASCII 码互转
来源：http://hz.nanxuanxn.top/gtnakcrkqu.html

Py:   ord("A"); chr(65)
来源：http://hz.zhoulong.xyz/gtmiyemagg.html

PHP:  ord("A"); chr(65)
来源：http://hz.hongshengwenyu.top/gtebitbear.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.birdmap.top/gtcodbqbyp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.iojbl.cn/gtsrjyafyt.html

Java: (int) 'A'; (char) 65
来源：http://hz.xuetiantiany.cn/gtdfndiejm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yuxming.cn/gtwzttppva.html

Ruby: "A".ord; 65.chr
来源：http://hz.gogol.net.cn/gtjkcsvpre.html

C#:   (int)'A'; (char)65
来源：http://hz.haohaochexian.top/gtxyhtquof.html

[A19] 交换两个变量
来源：http://hz.ehwqpu.com/gtfqpedltp.html

Py:   a, b = b, a
来源：http://hz.shuidangran.top/gtgvmwimxb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jinqigfzy.top/gtbznzfltu.html

JS:   [a, b] = [b, a];
来源：http://hz.jlsjyb.cn/gttgizwmmt.html

TS:   [a, b] = [b, a];
来源：http://hz.chenjidiqi.icu/gtnocuymus.html

Java: int t = a; a = b; b = t;
来源：http://hz.fengsongda.top/gtdenbfjxy.html

Go:   a, b = b, a
来源：http://hz.sweek.top/gtksaubaad.html

Ruby: a, b = b, a
来源：http://hz.shanyushiyangtech.top/gtgrwxbqmi.html

C#:   (a, b) = (b, a);
来源：http://hz.ehwqpu.com/gtavqhzigx.html

[A20] 读取标准输入
来源：http://hz.shzxlz.cn/gttmgscpgd.html

Py:   name = input("请输入：")
来源：http://hz.hnqzz.top/gtfzctkymo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.gogol.net.cn/gtcugobkgc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xziqi.cn/gttwzcapjj.html

TS:   // Node.js：readline 模块
来源：http://hz.yuanzhike.top/gtcuyyuxwf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.kuanghao11.cn/gtauzmvhzi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.fzhhl.top/gthrqparki.html

Ruby: gets.chomp
来源：http://hz.dashuyun.cn/gtqiskrhwy.html

C#:   Console.ReadLine();
来源：http://hz.shanyushiyangtech.top/gtdrzrrfjk.html

[A21] 保留指定小数位输出
来源：http://hz.gaohongyu789.top/gtjzpkebtl.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hfpthk.cn/gteahhdfjo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cashguo.top/gtxbzgiwob.html

JS:   (3.14159).toFixed(2)
来源：http://hz.mhx1999.top/gtczzuuicf.html

TS:   (3.14159).toFixed(2)
来源：http://hz.svipenyu.cn/gtnakfnxae.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ehwqpu.com/gtwexjbvdv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.sweek.top/gtfuckrgss.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtbbgiguie.html

C#:   3.14159.ToString("F2")
来源：http://hz.fzhhl.top/gthnfrxedi.html

[A22] 获取字符串长度
来源：http://hz.kuanghao11.cn/gtmhsbsdbe.html

Py:   len(s)
来源：http://hz.zhongyouzk.top/gtpkabgoud.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.sysykeji.top/gtclcybfkv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.shanyushiyangtech.top/gtxhdjgsps.html

TS:   s.length
来源：http://hz.zdqjudy.top/gthvjgffws.html

Java: s.length()
来源：http://hz.ppjwa.cn/gtbirybnnc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.quarkkingdee.top/gtflbrxluy.html

Ruby: s.length
来源：http://hz.chenzaomai.com/gtpyianwub.html

C#:   s.Length
来源：http://hz.shanyushiyangkeji.top/gtycajyjoy.html

[A23] 大小写转换
来源：http://hz.tian-w.cn/gtxqrzlwec.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.0kj1m.cn/gtyxrfmkyw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.c1oappe.top/gtdpltmheh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xylfe.cn/gtdveqktwu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnqzz.top/gtdvkkdpbl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yanxiufei.cn/gtkacuusop.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.shanyushiyangkeji.top/gtxdyvuyfl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.haohaochexian.top/gtyrchvphx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.hammf.cn/gteprkafbb.html

[A24] 去除首尾空白
来源：http://hz.xuanzx.com/gtridhwmiu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ivvv.top/gtsrobukbe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.birdmap.top/gtmosshgrl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhaomingkeji.xyz/gtyruczroq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigfzy.top/gtabcmlrxk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.mhx1999.top/gtivezvsfk.html

Go:   strings.TrimSpace(s)
来源：http://hz.feifeiyinyue.top/gtvqvnfaak.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xinyue.icu/gtrxejdzxc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.daria6918.cn/gtdrnuuyzu.html

[A25] 字符串比较
来源：http://hz.ywan-chungtsiang.top/gteovbwxqb.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yanxiufei.cn/gtpoqouvtp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.0kj1m.cn/gtfohjcmob.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tian-w.cn/gtrvgswzcf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.vqdsnc.cn/gtkctkjvgi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xylfe.cn/gtgiyragns.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yueranfly.top/gtobyhsrwp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ehwqpu.com/gtcvixrowx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.sweek.top/gtxuoikytc.html

[A26] 类型转换总览
来源：http://hz.tian-w.cn/gtdmsdznrq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ybcxt.top/gthgsxbbio.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.shangyingyoupin.top/gtjdnatsdh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.0kj1m.cn/gtfclwttcs.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jlsjyb.cn/gteephlwmt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.fengsongda.top/gtmizsqlqu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.nanxuanxn.top/gtffgrfyxw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.daxiang520.top/gtkfxctari.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhaomingkeji.xyz/gtfuqmdlyp.html

================================================================================
来源：http://hz.cashguo.top/gtywdbsuas.html

B. 流程控制
来源：http://hz.ehwqpu.com/gtbqevywvn.html

================================================================================
来源：http://hz.cashguo.top/gtjrsabptc.html

[B01] 条件判断 if / else
来源：http://hz.birdmap.top/gtjwuawcvq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.316326.xyz/gtdzmizlrr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zdqjudy.top/gthphuhabx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtlboawpid.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtnlievuxq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.redwolf501.top/gtoeakjnjd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.svipenyu.cn/gtqxrodfum.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gaohongyu789.top/gtxbvydiox.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtuitggxof.html

[B02] 多分支 else if / elif
来源：http://hz.meibo888.top/gtzilicpvj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yangfankeji.com/gtvopfjbkk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yueranfly.top/gtomlbmyzj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtyjbwryvn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtzklvpbri.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hysaishi.cn/gtdwrzpato.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yonumen.top/gtrytnnqtm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ydjk.org.cn/gtuwfijvov.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xingfuxueyuan.xyz/gtjcarkvgi.html

[B03] switch / match / case
来源：http://hz.xziqi.cn/gtlculqgao.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.redwolf501.top/gttzbpdmia.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.feifeiyinyue.top/gteihrcekh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenlongwang.top/gtdjnnmkwd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxinkj.top/gtpjpdrivh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.gaohongyu789.top/gtabtzdfmm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hfpthk.cn/gtfbgsourq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.xylfe.cn/gtuyzstohv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.chenlongwang.top/gtfpovvmkb.html

[B04] for 计数循环
来源：http://hz.yuanzhike.top/gtecasuvoo.html

Py:   for i in range(10): print(i)
来源：http://hz.52xcode.cn/gtcqmcaokw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gogol.net.cn/gtutghdbpx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtcqtjnzvz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yanxiufei.cn/gtugzajpeh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenzaomai.com/gtsgoahjad.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.mhx1999.top/gtyuybfsnp.html

Ruby: 10.times { |i| puts i }
来源：http://hz.bjfxy.top/gteexshxsd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.gzhubu.top/gtttbkbwdh.html

[B05] 遍历数组 / 列表
来源：http://hz.pengpengdd.cyou/gtigqcsshu.html

Py:   for item in arr: print(item)
来源：http://hz.zhaomingkeji.xyz/gtdyaoroqc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sweek.top/gtbuzpvqgz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.sweek.top/gtyabajwlu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.316326.xyz/gtzdnxcxtn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.vqdsnc.cn/gtndpubkwo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xylfe.cn/gtoupctbxy.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hnxiangtu.top/gtwdaouprm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj202588.top/gtzlpyvppt.html

[B06] 遍历字典 / 对象
来源：http://hz.jinghuilouyu.cn/gtnioexytc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhijiandao.cn/gtsqfmttnd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.bjfxy.top/gtmlgqejbs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pengpengdd.cyou/gttdkwbctn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sxryk.cn/gtuhvpitqk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shanyushiyangtech.top/gtueztrscg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hywenlv.cn/gtpeaiynon.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.mhx1999.top/gtufkcyddn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guannengcc.top/gtcqtgjjbb.html

[B07] while 循环
来源：http://hz.yvedp.cn/gttofdyjaz.html

Py:   while i < 10: i += 1
来源：http://hz.dianchejie.cn/gtnrwuvftp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fengsongda.top/gtvylggsqj.html

JS:   while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtutxdjjvv.html

TS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtmcrdwqkz.html

Java: while (i < 10) { i++; }
来源：http://hz.xziqi.cn/gtqjknshxa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xylfe.cn/gtysaiduml.html

Ruby: while i < 10; i += 1; end
来源：http://hz.daxiang520.top/gtpysqkjjm.html

C#:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtwrmojhfo.html

[B08] do-while（至少执行一次）
来源：http://hz.cqqwz.cn/gtqmpmhvuq.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhongyouzk.top/gtbgnhbtkn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.guannengcc.top/gtarvstsuo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gtmhlrcqfq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtmavjxngu.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtallwpoqa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ywan-chungtsiang.top/gtiggqcywz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jyoumei.cn/gtsfvuqesi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.wangshuangyany.cn/gtkbqvzmmh.html

[B09] break 与 continue
来源：http://hz.hongshengwenyu.top/gtngebdxsy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shangyingyoupin.top/gtbvwgzynj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.redwolf501.top/gtrapdyhca.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gthkboxoqv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtzoffjuaf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtkcmydlbh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.fengsongda.top/gthxfstiuu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.dianchejie.cn/gttrkwgjko.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtznpgyomp.html

[B10] 遍历同时拿索引
来源：http://hz.gaohongyu789.top/gtolblsxws.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dianchejie.cn/gtoiirfbqx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ehwqpu.com/gtleoofvpo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgfzy.top/gtsstpddnr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.daria6918.cn/gtykdgyjcx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guowangkeji.top/gtxvcierkt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.havefunace.top/gtqihzxkge.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tanke756.top/gtvnliflgw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hnqzz.top/gtxcsbnvxw.html

[B11] 生成数字序列 / 区间
来源：http://hz.hongshengwenyu.top/gthfajboux.html

Py:   list(range(0, 10, 2))
来源：http://hz.bjfxy.top/gtfntspfkp.html

PHP:  range(0, 10, 2);
来源：http://hz.svipenyu.cn/gtbkureddy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sufxvd.cn/gtptbkuvoy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtdubbuixr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gaohongyu789.top/gtsllradkc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258888.top/gtlhxytfgt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zycfv.cn/gtpcepwjme.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgufenzy.top/gtmkyhfqbt.html

[B12] 跳出多层循环
来源：http://hz.yangfankeji.com/gtiorsdxok.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.dashuyun.cn/gthagksijk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cashguo.top/gtcdjgzfuf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtkyableda.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtdqmwodik.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtwtkdeony.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cashguo.top/gtouvqcwgb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guowangkeji.top/gtpfmplnjw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yvedp.cn/gtwhfmsqaj.html

[B13] 判断是否为数字
来源：http://hz.xziqi.cn/gtbbrozgyz.html

Py:   isinstance(x, (int, float))
来源：http://hz.pycfn.com/gtasauhqww.html

PHP:  is_numeric($x)
来源：http://hz.meibo888.top/gtczjdnjqa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigfzy.top/gthzpfafho.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtwarwsxdm.html

Java: x instanceof Number
来源：http://hz.sxryk.cn/gteqzawxev.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yuxming.cn/gtjnnztiqx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhoulong.xyz/gtadsdsttj.html

C#:   x is int or double or decimal
来源：http://hz.hammf.cn/gtoyoqacii.html

[B14] 判断值是否在集合内
来源：http://hz.316326.xyz/gtfvoptmff.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jiagoushi.top/gtldajqxff.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinqigufen.top/gtryaziemy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhixingplan.top/gtlizivrck.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtkvperyom.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxuanxn.top/gtaglfvvpz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jiagoushi.top/gtqgjtprna.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zycfv.cn/gtbfvvkdio.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.daria6918.cn/gthwbhnvjv.html

[B15] 布尔运算与取反
来源：http://hz.cqqwz.cn/gtrcrymbdk.html

Py:   a and b or not c
来源：http://hz.zhijiandao.cn/gtfoaaxoxg.html

PHP:  $a && $b || !$c
来源：http://hz.hfpthk.cn/gtjxirfdzs.html

JS:   a && b || !c
来源：http://hz.c1oappe.top/gtyupaqvyv.html

TS:   a && b || !c
来源：http://hz.smart0.xyz/gtlmomkyid.html

Java: a && b || !c
来源：http://hz.jyoumei.cn/gtwaomjnfm.html

Go:   a && b || !c
来源：http://hz.tanke756.top/gtajpjuclq.html

Ruby: a && b || !c
来源：http://hz.xinyue.icu/gtbwupcnid.html

C#:   a && b || !c
来源：http://hz.nanxuanxn.top/gtawynyriy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xziqi.cn/gtzfbthrcx.html

Py:   if not data: return
来源：http://hz.quarkkingdee.top/gtngsjksfe.html

PHP:  if (!$data) { return; }
来源：http://hz.zycfv.cn/gtufmzxmsi.html

JS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtyqidgrvg.html

TS:   if (!data) return;
来源：http://hz.tian-w.cn/gtvogtwlfd.html

Java: if (data == null) return;
来源：http://hz.nanxinkj.top/gtvtqtperv.html

Go:   if data == nil { return }
来源：http://hz.nanxuanxn.top/gtdpfdhgph.html

Ruby: return if data.nil?
来源：http://hz.guowangkeji.top/gtbsjpsofd.html

C#:   if (data == null) return;
来源：http://hz.ybcxt.top/gtrkbhkecx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtynckbgzx.html

C. 函数与作用域
来源：http://hz.andypj.xyz/gthylxpztq.html

================================================================================
来源：http://hz.0kj1m.cn/gtcedeiyld.html

[C01] 定义函数
来源：http://hz.shanyushiyangtech.top/gtdxrlcpko.html

Py:   def add(a, b): return a + b
来源：http://hz.zycfv.cn/gtoahcqiwm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gtlgsenfyq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangdashe.top/gtexqfysit.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jiagoushi.top/gtyqghnwwh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtydfawspq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tian-w.cn/gtzxjdghra.html

Ruby: def add(a, b); a + b; end
来源：http://hz.quarkkingdee.top/gtpldnoqxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtjlghsffr.html

[C02] 默认参数
来源：http://hz.guowangkeji.top/gtdkscsxjd.html

Py:   def greet(name="World"): return name
来源：http://hz.aizwys.cn/gtvflybrhg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xziqi.cn/gteqlzsvff.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtngszlouv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtasckdfvl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj20258.top/gtpxjyfgjk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuanzx.com/gtbksqqemv.html

Ruby: def greet(name = "World") = name
来源：http://hz.c1oappe.top/gtavrnuafh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sxryk.cn/gtcsksrxeq.html

[C03] 可变参数
来源：http://hz.aibaodan.cn/gtxyyrwhsp.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtvgdzasmo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xingfuxueyuan.xyz/gttultanln.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gttfnaiouq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtfnwudluu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aibaodan.cn/gtvbpdayza.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xinyue.icu/gtgjxeobdx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tanke756.top/gtrvlcpzvm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtjlrwilqz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jianghu66.top/gtywxpmpqv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtqfubbvtr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pengpengdd.cyou/gtmxggdgjg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtxfiborak.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtklkkaqlm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuanzx.com/gtwfpgsmhw.html

Go:   // 无：用配置结构体参数
来源：http://hz.xylfe.cn/gtpievsifm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtjfgbfcoe.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gttjxfunsz.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtkrekzdxm.html

Py:   return a, b
来源：http://hz.316326.xyz/gtfpskhqyt.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtiatnjgws.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtrgyabkhb.html

TS:   return { a, b };
来源：http://hz.pengpengdd.cyou/gtmuhubnct.html


<!-- 参考信息 -->