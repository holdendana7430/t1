代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://hz.gaohongyu789.top/gtpcrncbeh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhengqikj.top/gtxolbpknx.html

Go:   // 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gtvpyykdbe.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jinghuilouyu.cn/gtrtxazdwd.html

C#:   // 单行；/* 多行 */
来源：http://hz.pengpengdd.cyou/gtmbeymhek.html

[A15] 空值判断与默认值
来源：http://hz.svipenyu.cn/gtgzxfmyms.html

Py:   value = data or "默认值"
来源：http://hz.xingfuxueyuan.xyz/gttigdorkk.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.birdmap.top/gthtxomcvw.html

JS:   const value = data ?? "默认值";
来源：http://hz.gotoacloud.top/gtxbisdube.html

TS:   const value = data ?? "默认值";
来源：http://hz.ywan-chungtsiang.top/gtjbbrxknj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.redwolf501.top/gtkuechaat.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.shanyushiyangtech.top/gtsworebnb.html

Ruby: value = data || "默认值"
来源：http://hz.tanke756.top/gtvjfybkbr.html

C#:   var value = data ?? "默认值";
来源：http://hz.feifeiyinyue.top/gtiambzpui.html

[A16] 真假值判断规则
来源：http://hz.chenzaomai.com/gtrnujotmu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.nwbrower.top/gtumtbqpan.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.wangshuangyany.cn/gtdpvxfksr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.gotoacloud.top/gtpkzcotwm.html

TS:   if (!x) {}
来源：http://hz.zdqjudy.top/gthohibpfm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yonumen.top/gtvcfggkns.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.xuanzx.com/gtsusakjxm.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.sysykeji.top/gtskbzfdll.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.smart0.xyz/gtsekihdfk.html

[A17] 位运算
来源：http://hz.cdnleiting.top/gtpcgoqwhd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtmmjlbnqi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ehwqpu.com/gtynfpbrma.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gotoacloud.top/gtibjrefbd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.nanxinkj.top/gtjxaczxuq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtelojiqdf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gthfrllcbd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtyppvbalx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gtinjrdvjz.html

[A18] 字符与 ASCII 码互转
来源：http://hz.smart0.xyz/gtgbmqugdf.html

Py:   ord("A"); chr(65)
来源：http://hz.gotoacloud.top/gtammtqqal.html

PHP:  ord("A"); chr(65)
来源：http://hz.ehwqpu.com/gtkatbhizd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yonumen.top/gtnqxkwrwa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sufxvd.cn/gtprhkucwh.html

Java: (int) 'A'; (char) 65
来源：http://hz.xinyue.icu/gtiofmnccv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xinyue.icu/gtbwvrrnet.html

Ruby: "A".ord; 65.chr
来源：http://hz.smart0.xyz/gtxawiwxhw.html

C#:   (int)'A'; (char)65
来源：http://hz.wangdashe.top/gttuyymexo.html

[A19] 交换两个变量
来源：http://hz.52xcode.cn/gthwdopjpt.html

Py:   a, b = b, a
来源：http://hz.fengsongda.top/gtpgacwtep.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.guowangkeji.top/gtcxxqcmin.html

JS:   [a, b] = [b, a];
来源：http://hz.jinyuanbaomall.cn/gtmkpjysxk.html

TS:   [a, b] = [b, a];
来源：http://hz.hfpthk.cn/gtllqkmcxd.html

Java: int t = a; a = b; b = t;
来源：http://hz.zhiwuduotai.top/gtnhhmqitp.html

Go:   a, b = b, a
来源：http://hz.hfpthk.cn/gtzxgppymu.html

Ruby: a, b = b, a
来源：http://hz.sxryk.cn/gtrwochran.html

C#:   (a, b) = (b, a);
来源：http://hz.shanyushiyangkeji.top/gtudfwmwyh.html

[A20] 读取标准输入
来源：http://hz.kuanghao11.cn/gtviyrqcdj.html

Py:   name = input("请输入：")
来源：http://hz.wangdashe.top/gtybopxrey.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yueranfly.top/gtdpwlskii.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.guowangkeji.top/gtitrzlxrh.html

TS:   // Node.js：readline 模块
来源：http://hz.yj202588.top/gtcnpgdgdb.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.fzhhl.top/gtazakzbch.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.c1oappe.top/gtzuxosfym.html

Ruby: gets.chomp
来源：http://hz.cucudq.cn/gtdwzuvqvc.html

C#:   Console.ReadLine();
来源：http://hz.nanxinkj.top/gtguctrjbb.html

[A21] 保留指定小数位输出
来源：http://hz.nwbrower.top/gteaksfvfx.html

Py:   f"{3.14159:.2f}"
来源：http://hz.316326.xyz/gtuxvdciqj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.haohaochexian.top/gtpugwmcyp.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xziqi.cn/gtrionpnrs.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sysykeji.top/gtjgotcgea.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.0kj1m.cn/gtxhdixtcj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtjyfgxaqz.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtodtwfovg.html

C#:   3.14159.ToString("F2")
来源：http://hz.tian-w.cn/gtcrrruocr.html

[A22] 获取字符串长度
来源：http://hz.birdmap.top/gtkmotixdy.html

Py:   len(s)
来源：http://hz.tian-w.cn/gtezgoivns.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xziqi.cn/gtbkgxcpsu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xuetiantiany.cn/gtdxjdrhmw.html

TS:   s.length
来源：http://hz.hysaishi.cn/gtwwtutuam.html

Java: s.length()
来源：http://hz.iojbl.cn/gtclmumagv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.c1oappe.top/gtaaertfka.html

Ruby: s.length
来源：http://hz.hongshengwenyu.top/gtewllgrlm.html

C#:   s.Length
来源：http://hz.jyoumei.cn/gtqbqtageu.html

[A23] 大小写转换
来源：http://hz.guowangkeji.top/gtfhjrxlde.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ehwqpu.com/gtfwlofrfu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.aibaodan.cn/gtlgvqnbsy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhiwuduotai.top/gtogyffuio.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jqgufenzy.top/gtytodnxlp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenjidiqi.icu/gtsnbidnzy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.9152youxi.cn/gtwhvdnbns.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.cdnleiting.top/gtrbguvfuw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.c1oappe.top/gtpjvktmzj.html

[A24] 去除首尾空白
来源：http://hz.yueranfly.top/gtfezzzunj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.316326.xyz/gtsayhjynp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yuxming.cn/gthyhhfltl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cashguo.top/gtgwnfexxd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zdqjudy.top/gtakkeyajk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ydzc1.top/gtmtfxftii.html

Go:   strings.TrimSpace(s)
来源：http://hz.aizwys.cn/gtwsylrwcp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sxryk.cn/gtchlhlzbi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ppjwa.cn/gtfmkyzoss.html

[A25] 字符串比较
来源：http://hz.hammf.cn/gtwhqujamq.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cdnleiting.top/gtphjmotoj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.nwbrower.top/gtpcnnzrqs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xinyue.icu/gtmaujyzee.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuanzhike.top/gtcvjiygkr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zycfv.cn/gtkfzxfarl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhaomingkeji.xyz/gtizvxpwks.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.wangdashe.top/gtyvuzuqjw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.tian-w.cn/gtammpsjde.html

[A26] 类型转换总览
来源：http://hz.dianchejie.cn/gtqicumhzb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.tian-w.cn/gthzrydnab.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.havefunace.top/gtyiigwaii.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhiwuduotai.top/gtzycmdegq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sxryk.cn/gtrstrjlmt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shuidangran.top/gtrdjmdgyo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.smart0.xyz/gtyhhipxtf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.vqdsnc.cn/gtelgrfkyf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhongyouzk.top/gtzwlynuli.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmxypdvis.html

B. 流程控制
来源：http://hz.yuxming.cn/gtxmexsgni.html

================================================================================
来源：http://hz.shuidangran.top/gtxcbjezch.html

[B01] 条件判断 if / else
来源：http://hz.ybcxt.top/gtqkmpdjsj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.0kj1m.cn/gthpratnyf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.c1oappe.top/gtfpyvmlry.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yonumen.top/gtymguqxeb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhoulong.xyz/gtrkipfpxh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.chenzaomai.com/gtjehtmany.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ydjk.org.cn/gtmoczexph.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhiwuduotai.top/gttwmjhrmn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gtxjnqldyf.html

[B02] 多分支 else if / elif
来源：http://hz.svipenyu.cn/gtzbbiplwk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.dianchejie.cn/gtmcfmvphx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yonumen.top/gtckhwrzll.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtfqexdjuk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtldtuzxel.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.mhx1999.top/gtjgzlmrof.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yueranfly.top/gtjzfkecpq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.wangshuangyany.cn/gtneitagha.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtvzmqauis.html

[B03] switch / match / case
来源：http://hz.guannengcc.top/gtdzdmpqec.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cqqwz.cn/gthsdefhqf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shzxlz.cn/gtspbtdpco.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shuidangran.top/gtlzjbkihu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xziqi.cn/gtcceaheop.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yvedp.cn/gtodewzjhr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jyoumei.cn/gtpmtsskcv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shanyushiyangkeji.top/gtfpljtpge.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.shzxlz.cn/gtnydsarpj.html

[B04] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtknmscugj.html

Py:   for i in range(10): print(i)
来源：http://hz.sxryk.cn/gtxurkdarw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xuetiantiany.cn/gtsyhjrqbz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhongyouzk.top/gtnoyvkgpc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.9152youxi.cn/gtnhdlswud.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenlongwang.top/gthnkctoau.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinyuanbaomall.cn/gtobsusbig.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cashguo.top/gthzsvucey.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jqgufenzy.top/gtkjbzaykj.html

[B05] 遍历数组 / 列表
来源：http://hz.fengsongda.top/gtnpudwuvb.html

Py:   for item in arr: print(item)
来源：http://hz.zhaomingkeji.xyz/gtecncnsin.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.daxiang520.top/gtsfihkvbb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.daria6918.cn/gtmibqjyvk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.guowangkeji.top/gtekpfapgy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.meibo888.top/gtmmozejiq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnxiangtu.top/gtxaxupiwo.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yangfankeji.com/gtrxdvlnmc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.dashuyun.cn/gtzgpozfkz.html

[B06] 遍历字典 / 对象
来源：http://hz.redwolf501.top/gtfuimglra.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258.top/gtozpsfxtp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.redwolf501.top/gtzotppzij.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgfzy.top/gtzfmbhurq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtivhqrvbr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.guannengcc.top/gtdhzpozlo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.andypj.xyz/gtiihcebtg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhoulong.xyz/gtjtzfobgu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ehwqpu.com/gtkzjjcaxi.html

[B07] while 循环
来源：http://hz.yongpay.top/gtqhovlczk.html

Py:   while i < 10: i += 1
来源：http://hz.hammf.cn/gtgtfmgoeq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.dashuyun.cn/gthekdmkbf.html

JS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gteksrokxx.html

TS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtnwgubkgz.html

Java: while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtbudbzlfs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gogol.net.cn/gtoybsjlbl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnxiangtu.top/gtaumolrwj.html

C#:   while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtmtxwyjlx.html

[B08] do-while（至少执行一次）
来源：http://hz.aizwys.cn/gteotctles.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ywan-chungtsiang.top/gtkasxpywq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sysykeji.top/gtvtmqqkfm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tian-w.cn/gtiisflqkp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtykizgxuv.html

Java: do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtncsxozqn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.quarkkingdee.top/gtyreeqpfg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shangyingyoupin.top/gttchzogbf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gttpowcfil.html

[B09] break 与 continue
来源：http://hz.hnxiangtu.top/gtavjhnhzj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.snrcjt.cn/gtkbjyifeb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.dianchejie.cn/gtrfqzwfkh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtpwobkuoe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gthzkooltl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fengsongda.top/gtqjfacltf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.fzhhl.top/gtewhefavr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jiagoushi.top/gtcuanjzfz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtqpkbhrgi.html

[B10] 遍历同时拿索引
来源：http://hz.yj202588.top/gtjjopbmfj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.smart0.xyz/gtbwvyzprb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.aizwys.cn/gtjqgjpksi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jlsjyb.cn/gtrtkesrdz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj20258.top/gtivtienlb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tianlin.xyz/gtjbsgfohb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gaohongyu789.top/gtisvqunnq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yongpay.top/gtpvloivrj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jlsjyb.cn/gtxhqxeduo.html

[B11] 生成数字序列 / 区间
来源：http://hz.yanxiufei.cn/gtabwnhhao.html

Py:   list(range(0, 10, 2))
来源：http://hz.tianlin.xyz/gticymusfq.html

PHP:  range(0, 10, 2);
来源：http://hz.jyoumei.cn/gtpcewzllq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj202588.top/gtbgdvtekf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jianghu66.top/gtnjlhrgfu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aizwys.cn/gtslvepfti.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigufen.top/gtbtywgxrs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhiwuduotai.top/gtwtdwzqrj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj20258.top/gtgipoxbgy.html

[B12] 跳出多层循环
来源：http://hz.c1oappe.top/gtbnghswgh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tianlin.xyz/gtybqshpxa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnxiangtu.top/gtqahtlhkj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtpuanlnfg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtdwciuwcm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtpuwvatyb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtwvznrxjv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jqgufenzy.top/gtcmawhtzi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gtjracmzyr.html

[B13] 判断是否为数字
来源：http://hz.svipenyu.cn/gteuuxqtok.html

Py:   isinstance(x, (int, float))
来源：http://hz.mhx1999.top/gtprvbbdgb.html

PHP:  is_numeric($x)
来源：http://hz.ydjk.org.cn/gtudzelffi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtaossfjtr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gttirpjbhs.html

Java: x instanceof Number
来源：http://hz.gogol.net.cn/gtjzkhqjrz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jyoumei.cn/gtiybxnmlt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhiwuduotai.top/gttsyehbih.html

C#:   x is int or double or decimal
来源：http://hz.ybcxt.top/gtqmpfbxtt.html

[B14] 判断值是否在集合内
来源：http://hz.smart0.xyz/gtnpiqudmf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jqgfzy.top/gttiayafze.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.haohaochexian.top/gtymutgkaf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtdpyonxuv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.fzhhl.top/gtjkgrxwda.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.wangshuangyany.cn/gtntcjdzop.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yangfankeji.com/gtplndlgfx.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.0kj1m.cn/gtmeuzyyxg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.pengpengdd.cyou/gtkrnndprn.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gtkfyvuuxj.html

Py:   a and b or not c
来源：http://hz.zhiwuduotai.top/gtywroosue.html

PHP:  $a && $b || !$c
来源：http://hz.gzhubu.top/gtwatonkyv.html

JS:   a && b || !c
来源：http://hz.yongpay.top/gtxaspmmmm.html

TS:   a && b || !c
来源：http://hz.xuanzx.com/gtpesnhgkn.html

Java: a && b || !c
来源：http://hz.ydjk.org.cn/gtfcriuxde.html

Go:   a && b || !c
来源：http://hz.sweek.top/gtmaoczozj.html

Ruby: a && b || !c
来源：http://hz.zhijiandao.cn/gtwwdgotpe.html

C#:   a && b || !c
来源：http://hz.yanxiufei.cn/gtxuujiomb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gtcbdqyxue.html

Py:   if not data: return
来源：http://hz.yongpay.top/gtyncivtzf.html

PHP:  if (!$data) { return; }
来源：http://hz.ppjwa.cn/gtmsprnjxm.html

JS:   if (!data) return;
来源：http://hz.hywenlv.cn/gtsnfidfdq.html

TS:   if (!data) return;
来源：http://hz.pengpengdd.cyou/gtkqdbslml.html

Java: if (data == null) return;
来源：http://hz.zhongyouzk.top/gtmpxexkvc.html

Go:   if data == nil { return }
来源：http://hz.yvedp.cn/gtgblhvjrr.html

Ruby: return if data.nil?
来源：http://hz.c1oappe.top/gtovikhwdk.html

C#:   if (data == null) return;
来源：http://hz.xuanzx.com/gtnhoqnqdf.html

================================================================================
来源：http://hz.cheryme.top/gtqefqsemz.html

C. 函数与作用域
来源：http://hz.xziqi.cn/gtqzfodjja.html

================================================================================
来源：http://hz.cashguo.top/gtqtylhfjc.html

[C01] 定义函数
来源：http://hz.tianlin.xyz/gtkhmpgphf.html

Py:   def add(a, b): return a + b
来源：http://hz.sxryk.cn/gtgozyneoi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtlbbfadlh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigufen.top/gtuytwolli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtkajvjjqv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtslggttvu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.haohaochexian.top/gtgnqsundh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ehwqpu.com/gtiojkwymz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtivpkaskp.html

[C02] 默认参数
来源：http://hz.bjfxy.top/gtklktpowj.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangtech.top/gtoetdhufj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinghuilouyu.cn/gtqoeugzbn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtizpxbywh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.andypj.xyz/gtiakxgpnd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gaohongyu789.top/gtwipzuxsw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.vqdsnc.cn/gtmcqbgodj.html

Ruby: def greet(name = "World") = name
来源：http://hz.bjfxy.top/gtggvfywip.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigufen.top/gtbcnzkebu.html

[C03] 可变参数
来源：http://hz.yj20258.top/gtxgkbdhso.html

Py:   def total(*args): return sum(args)
来源：http://hz.guannengcc.top/gtytkwlrrg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtwtfyjxvb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtdjjcvufo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gtoybmeypu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtnnybimxz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.mhx1999.top/gtmziaajkt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yonumen.top/gtflestxln.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jianghu66.top/gtukztpjkc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ywan-chungtsiang.top/gtzoyasuku.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenjidiqi.icu/gtotwbirvu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tian-w.cn/gtiflvzbtf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtnfdqmijc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.c1oappe.top/gtndpflmya.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guowangkeji.top/gtajwajask.html

Go:   // 无：用配置结构体参数
来源：http://hz.pycfn.com/gtggqzjmnp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtoybvwrxr.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtyfivqxxu.html

[C05] 返回多个值
来源：http://hz.svipenyu.cn/gtzpzqjrwt.html


<!-- 参考信息 -->