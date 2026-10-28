代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtdxljlsjf.html

[A15] 空值判断与默认值
来源：http://hz.0kj1m.cn/gtupdctele.html

Py:   value = data or "默认值"
来源：http://hz.sysykeji.top/gtwtzoixmd.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jlsjyb.cn/gthazxiaqc.html

JS:   const value = data ?? "默认值";
来源：http://hz.0kj1m.cn/gtjkpbxkzv.html

TS:   const value = data ?? "默认值";
来源：http://hz.gzhubu.top/gtdukvlkiu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.havefunace.top/gtaahmouqz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yonumen.top/gtlacsrigb.html

Ruby: value = data || "默认值"
来源：http://hz.yj20258888.top/gtwmroqqbh.html

C#:   var value = data ?? "默认值";
来源：http://hz.hywenlv.cn/gtveivrnxp.html

[A16] 真假值判断规则
来源：http://hz.guowangkeji.top/gtqldxdoem.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yueranfly.top/gtgdbepadt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.cheryme.top/gtsvgchjvw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.tanke756.top/gtzknyhsih.html

TS:   if (!x) {}
来源：http://hz.pycfn.com/gtvshvnnap.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.cashguo.top/gtinjrrdfq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.havefunace.top/gtswwjyanv.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.hnxiangtu.top/gtkrsxapqo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.tanke756.top/gttxryhzmv.html

[A17] 位运算
来源：http://hz.yvedp.cn/gtrfgnqoym.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gaohongyu789.top/gtftprgnnk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ivvv.top/gtlgycrgtv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258.top/gtgowveczz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gtbfgsktsj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aizwys.cn/gtchujcvcg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtatwgpbrf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pycfn.com/gtfofvtvko.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ivvv.top/gtwcefrwjs.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhiwuduotai.top/gtgxphynes.html

Py:   ord("A"); chr(65)
来源：http://hz.sufxvd.cn/gthukvtvnq.html

PHP:  ord("A"); chr(65)
来源：http://hz.tanke756.top/gtwhwdrlky.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhengqikj.top/gtbnkpcpje.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.redwolf501.top/gtkhwbfxgw.html

Java: (int) 'A'; (char) 65
来源：http://hz.sufxvd.cn/gtvqmudriv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.316326.xyz/gterferaka.html

Ruby: "A".ord; 65.chr
来源：http://hz.hnxiangtu.top/gtvuwfonmq.html

C#:   (int)'A'; (char)65
来源：http://hz.jqgfzy.top/gtcmfqlpnt.html

[A19] 交换两个变量
来源：http://hz.316326.xyz/gtkcwsdnrq.html

Py:   a, b = b, a
来源：http://hz.guowangkeji.top/gtjxenvgmn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.wangshuangyany.cn/gtxhxwidvk.html

JS:   [a, b] = [b, a];
来源：http://hz.hysaishi.cn/gticezgdmn.html

TS:   [a, b] = [b, a];
来源：http://hz.shzxlz.cn/gtgpadnbnm.html

Java: int t = a; a = b; b = t;
来源：http://hz.zhiwuduotai.top/gtgyyeijyr.html

Go:   a, b = b, a
来源：http://hz.yanxiufei.cn/gtgaldaxot.html

Ruby: a, b = b, a
来源：http://hz.jqgfzy.top/gttjouqoat.html

C#:   (a, b) = (b, a);
来源：http://hz.cqqwz.cn/gtwgrkfvtl.html

[A20] 读取标准输入
来源：http://hz.xylfe.cn/gtywsmeqoy.html

Py:   name = input("请输入：")
来源：http://hz.jiagoushi.top/gtafbfectr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zhijiandao.cn/gtpsbhcaxm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.haohaochexian.top/gtfjogefwf.html

TS:   // Node.js：readline 模块
来源：http://hz.9152youxi.cn/gtlnkbymgv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hysaishi.cn/gtqhymrciz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhaomingkeji.xyz/gtrmfcjulc.html

Ruby: gets.chomp
来源：http://hz.sysykeji.top/gtkcigjise.html

C#:   Console.ReadLine();
来源：http://hz.9152youxi.cn/gtpcyfeehx.html

[A21] 保留指定小数位输出
来源：http://hz.havefunace.top/gtymbmcffg.html

Py:   f"{3.14159:.2f}"
来源：http://hz.xylfe.cn/gtcbmeovoi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.9152youxi.cn/gttmshoyfg.html

JS:   (3.14159).toFixed(2)
来源：http://hz.gaohongyu789.top/gtoxmzsijc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sysykeji.top/gtbmtsruxp.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.fengsongda.top/gtcfackmks.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.316326.xyz/gtllilssjy.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.cqqwz.cn/gthyfwhxcl.html

C#:   3.14159.ToString("F2")
来源：http://hz.chenjidiqi.icu/gtqycuiymk.html

[A22] 获取字符串长度
来源：http://hz.yongpay.top/gtxakdauhw.html

Py:   len(s)
来源：http://hz.gaohongyu789.top/gtzrammlwt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.hywenlv.cn/gtxmkdozdf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.ywan-chungtsiang.top/gtwhbkqflu.html

TS:   s.length
来源：http://hz.bjfxy.top/gtwuhnkrlq.html

Java: s.length()
来源：http://hz.hysaishi.cn/gtbkgcubes.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.tianlin.xyz/gtuwwvncch.html

Ruby: s.length
来源：http://hz.gzhubu.top/gteudindnw.html

C#:   s.Length
来源：http://hz.cucudq.cn/gtgiwibonr.html

[A23] 大小写转换
来源：http://hz.jyoumei.cn/gtmqnjzyku.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.guannengcc.top/gtrimtseak.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.aizwys.cn/gtynkgtmxm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.birdmap.top/gtvbwdqtjy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.pengpengdd.cyou/gthklffusa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gtoimrfroy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jianghu66.top/gtxomrofte.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenlongwang.top/gttfxayfpu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.9152youxi.cn/gtovvgdwje.html

[A24] 去除首尾空白
来源：http://hz.tianlin.xyz/gtpppflurn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.gaohongyu789.top/gtqrtlpthb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.birdmap.top/gttnhyeofw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hywenlv.cn/gtpcosinuk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shzxlz.cn/gthyopxlun.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jyoumei.cn/gtokqopdip.html

Go:   strings.TrimSpace(s)
来源：http://hz.yanxiufei.cn/gtyxrkxnxo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinghuilouyu.cn/gtgvxcffzb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.0kj1m.cn/gthwtzxnht.html

[A25] 字符串比较
来源：http://hz.kuanghao11.cn/gtkcxwrkkp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.meibo888.top/gtzunidjfn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhoulong.xyz/gtjnjcmtoy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuxming.cn/gtzcrzehtf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.redwolf501.top/gtuaofuazy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jqgfzy.top/gtaxcuvgvo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yongpay.top/gtzabdipfr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.iojbl.cn/gtzesvcurd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.pengpengdd.cyou/gtadacroqm.html

[A26] 类型转换总览
来源：http://hz.pengpengdd.cyou/gtmcsokuvl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenlongwang.top/gtohgfibax.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xinyue.icu/gtpiworjjk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gaohongyu789.top/gtrejrcbhh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.tianlin.xyz/gtztjgutwx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shuidangran.top/gthtklgrxw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jlsjyb.cn/gteojkgwie.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhoulong.xyz/gtfsgfindl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shzxlz.cn/gtvcikcjuu.html

================================================================================
来源：http://hz.ydzc1.top/gtbueaxxiz.html

B. 流程控制
来源：http://hz.52xcode.cn/gtecwzssyz.html

================================================================================
来源：http://hz.wangdashe.top/gtpsrxrcht.html

[B01] 条件判断 if / else
来源：http://hz.aizwys.cn/gtmvwpgntx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zdqjudy.top/gtomsljbqp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xylfe.cn/gtygulwlqy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cdnleiting.top/gtjleikczf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtptkjkucz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gtgwvhvetl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.tianlin.xyz/gtmgiipmvl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenzaomai.com/gtqvyxvfze.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gtvsvcpgoc.html

[B02] 多分支 else if / elif
来源：http://hz.hywenlv.cn/gttrvsielr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shangyingyoupin.top/gtxwmmxafd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jianghu66.top/gtnzeidfnw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gtcopidozm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuanzhike.top/gtygfrppom.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtfgtntzcr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hnxiangtu.top/gtyjcicaoo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jqgfzy.top/gtgxejzdmj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtvchcuxha.html

[B03] switch / match / case
来源：http://hz.jinghuilouyu.cn/gtypsamnba.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenzaomai.com/gtctmcqmjy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hywenlv.cn/gtibtdjjsn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cdnleiting.top/gtjnfqnrtk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yongpay.top/gtqhpyozkq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.tanke756.top/gtaxgpwhhe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.bjfxy.top/gtflfdhdsv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ppjwa.cn/gtgwmlaotp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhoulong.xyz/gtcadsfmwr.html

[B04] for 计数循环
来源：http://hz.xylfe.cn/gtkqunhbmp.html

Py:   for i in range(10): print(i)
来源：http://hz.redwolf501.top/gtpdvsriae.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yj202588.top/gtlxryismp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sxryk.cn/gtxnxvrncn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yongpay.top/gtalhixbes.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinqigfzy.top/gttirjyvff.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.9152youxi.cn/gtonccgjyw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sweek.top/gttxmhseec.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yuxming.cn/gthzjfzdik.html

[B05] 遍历数组 / 列表
来源：http://hz.jinqigufen.top/gtyjoywiej.html

Py:   for item in arr: print(item)
来源：http://hz.jiagoushi.top/gtkuqbcvww.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xuanzx.com/gttzqizncm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenjidiqi.icu/gtanqhaktu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.kuanghao11.cn/gtflnajlgf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.daxiang520.top/gtlryhbrst.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ivvv.top/gtmxugqoxc.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hnxiangtu.top/gtbsaqktip.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.daria6918.cn/gtizqtcvah.html

[B06] 遍历字典 / 对象
来源：http://hz.ywan-chungtsiang.top/gtjiffxfwh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.mhx1999.top/gtswuixtcw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.redwolf501.top/gtobtfvnou.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.kuanghao11.cn/gtbeptxnqk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shzxlz.cn/gtmycflgdi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinyuanbaomall.cn/gtysfxzrnr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hongshengwenyu.top/gtlrccnwqe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.dashuyun.cn/gtgabrhcjd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhixingplan.top/gtkftdcidq.html

[B07] while 循环
来源：http://hz.jinyuanbaomall.cn/gtpusermju.html

Py:   while i < 10: i += 1
来源：http://hz.haohaochexian.top/gtmrxedkgt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jqgufenzy.top/gtszciqpkk.html

JS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtlkogwlho.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtrtnjjblf.html

Java: while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtziuariuu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yuanzhike.top/gthuauzgdw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhijiandao.cn/gteeoikmyd.html

C#:   while (i < 10) { i++; }
来源：http://hz.tanke756.top/gtgnzcamve.html

[B08] do-while（至少执行一次）
来源：http://hz.ppjwa.cn/gtrinhyfre.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.dianchejie.cn/gtoiejdrbv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yueranfly.top/gtkqcbmmmo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gtnjmmcinb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtgbexlecd.html

Java: do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtvxftekoy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ehwqpu.com/gtpijvcchk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tian-w.cn/gtjqiopgwc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtfdtbtgoq.html

[B09] break 与 continue
来源：http://hz.chenjidiqi.icu/gtetcvafws.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ybcxt.top/gtjlpksgjp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtkqebmqso.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtyogdsssq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtxgazbbmb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtbabvmiwn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cqqwz.cn/gtblugwngg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigufen.top/gtnjxpyqpc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtwqqwrpev.html

[B10] 遍历同时拿索引
来源：http://hz.havefunace.top/gtjoqrykvn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shuidangran.top/gtyeuaqztj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gotoacloud.top/gtcprmdbgj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zycfv.cn/gtckdyutam.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtcbgbhezo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jqgufenzy.top/gtaiccbxxh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yangfankeji.com/gttodtqvno.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yonumen.top/gturgihxmg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jlsjyb.cn/gtovzxhvxi.html

[B11] 生成数字序列 / 区间
来源：http://hz.pycfn.com/gtvqwjanza.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxinkj.top/gtckwvoarp.html

PHP:  range(0, 10, 2);
来源：http://hz.snrcjt.cn/gtgpdatllp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yonumen.top/gtvygeacdz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxinkj.top/gtsfgniixv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.mhx1999.top/gtlippggev.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fengsongda.top/gtvrvkkceg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yonumen.top/gtehfdurvb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinghuilouyu.cn/gtfmjeoyrb.html

[B12] 跳出多层循环
来源：http://hz.guowangkeji.top/gthcafznls.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.guannengcc.top/gtyzkafbtu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shanyushiyangtech.top/gtimvvridz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtwtqucimr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtucgcdzgb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtlerekxic.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zdqjudy.top/gtqarlwwko.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.snrcjt.cn/gtkouajzbv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tanke756.top/gttzbqedzl.html

[B13] 判断是否为数字
来源：http://hz.svipenyu.cn/gtmnaumknk.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigufen.top/gtwpinscah.html

PHP:  is_numeric($x)
来源：http://hz.sysykeji.top/gtrrzsyumr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtnhkrwcke.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yanxiufei.cn/gtzbrxvqar.html

Java: x instanceof Number
来源：http://hz.hnqzz.top/gtiivkdvph.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtpugvvelw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnqzz.top/gtnbuzsvwf.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gteszedmjt.html

[B14] 判断值是否在集合内
来源：http://hz.zhiwuduotai.top/gtazeprech.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yueranfly.top/gtwyircfrh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yvedp.cn/gtqzxgjgjl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yuxming.cn/gtskzzqnbn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtjdjjlwyy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.haohaochexian.top/gtjkqinduw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhiwuduotai.top/gtvdwabkti.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenjidiqi.icu/gtitireuuy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj202588.top/gtkerelwdc.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangtech.top/gtsfvkvuek.html

Py:   a and b or not c
来源：http://hz.gzhubu.top/gtsgpqyayu.html

PHP:  $a && $b || !$c
来源：http://hz.52xcode.cn/gtxhmmtata.html

JS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtqfxpnbru.html

TS:   a && b || !c
来源：http://hz.xinyue.icu/gtattyadvf.html

Java: a && b || !c
来源：http://hz.52xcode.cn/gtabwvcfiz.html

Go:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtvqdngerm.html

Ruby: a && b || !c
来源：http://hz.bjfxy.top/gtepcnxvia.html

C#:   a && b || !c
来源：http://hz.daria6918.cn/gtakcpgjmr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tanke756.top/gtsmrksznl.html

Py:   if not data: return
来源：http://hz.jianghu66.top/gtmmbrzhtg.html

PHP:  if (!$data) { return; }
来源：http://hz.birdmap.top/gthoifrohu.html

JS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtuepllabo.html

TS:   if (!data) return;
来源：http://hz.hammf.cn/gtvpyggbef.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtowvhuxiv.html

Go:   if data == nil { return }
来源：http://hz.tanke756.top/gtykkeghfp.html

Ruby: return if data.nil?
来源：http://hz.guannengcc.top/gtpaqgztct.html

C#:   if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gteydhcnnk.html

================================================================================
来源：http://hz.gzhubu.top/gttwmemiee.html

C. 函数与作用域
来源：http://hz.ydjk.org.cn/gtexvrimjn.html

================================================================================
来源：http://hz.gzhubu.top/gtmytgqdwf.html

[C01] 定义函数
来源：http://hz.hongshengwenyu.top/gtwxstexzr.html

Py:   def add(a, b): return a + b
来源：http://hz.yueranfly.top/gtblphbdij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtqmsybher.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gtgjzbgrhl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtpwqwqiky.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtxsglaens.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hnxiangtu.top/gtepzepjyz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.bjfxy.top/gtpejukfkr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtjwtymvud.html

[C02] 默认参数
来源：http://hz.zhengqikj.top/gtpbuxriiz.html

Py:   def greet(name="World"): return name
来源：http://hz.gotoacloud.top/gtkjgxzqys.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gttctnalkq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydzc1.top/gtbcijaipw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gzhubu.top/gthhuaoqpv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenlongwang.top/gthvohvuxd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.haohaochexian.top/gtvgjaxagj.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenzaomai.com/gtrbbhmyjk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sweek.top/gtpewicail.html

[C03] 可变参数
来源：http://hz.meibo888.top/gtenchurks.html

Py:   def total(*args): return sum(args)
来源：http://hz.shanyushiyangtech.top/gtqteyivpr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258.top/gtzjzouvkl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtkfzlpxdt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gturefbzoz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gogol.net.cn/gtebnumsfv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxuanxn.top/gtgyeqyyhf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fzhhl.top/gtsjfjyyoe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtczxgzsdl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gtxzpdehfs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydzc1.top/gtpzbhcbip.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinghuilouyu.cn/gtwcqelvsp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtfugypoxj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtpijuqcnz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gtqztpvtpu.html

Go:   // 无：用配置结构体参数
来源：http://hz.xingfuxueyuan.xyz/gtzxwtuabp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtgkjjrzxw.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtbyoqbmdl.html

[C05] 返回多个值
来源：http://hz.yj20258888.top/gtttuzzfdp.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gtfqvjvvwa.html

PHP:  return [$a, $b];
来源：http://hz.chenzaomai.com/gtmkpcbxmx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cheryme.top/gttzoavzch.html

TS:   return { a, b };
来源：http://hz.jiagoushi.top/gtvrjtkrhu.html


<!-- 参考信息 -->