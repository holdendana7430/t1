代发 wailian999

[A14] 注释写法
来源：http://hz.xingfuxueyuan.xyz/gtthvcbdjm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hongshengwenyu.top/gtbsuifwab.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.havefunace.top/gtpmofkzmu.html

JS:   // 单行；/* 多行 */
来源：http://hz.fzhhl.top/gtanrvpyik.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhixingplan.top/gtzscwcewm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.hnxiangtu.top/gtjlbruqkc.html

Go:   // 单行；/* 多行 */
来源：http://hz.jinghuilouyu.cn/gtjdgzetwk.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.havefunace.top/gtdhccmnto.html

C#:   // 单行；/* 多行 */
来源：http://hz.pengpengdd.cyou/gtejdpvgxl.html

[A15] 空值判断与默认值
来源：http://hz.52xcode.cn/gtzvjoxeal.html

Py:   value = data or "默认值"
来源：http://hz.yangfankeji.com/gtchhcnuxr.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.cqqwz.cn/gtillzqrwy.html

JS:   const value = data ?? "默认值";
来源：http://hz.nanxuanxn.top/gtvikplovh.html

TS:   const value = data ?? "默认值";
来源：http://hz.gogol.net.cn/gtrpdfbydd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.ivvv.top/gtpohgkvsg.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.tianlin.xyz/gtrycbngeq.html

Ruby: value = data || "默认值"
来源：http://hz.gogol.net.cn/gtteexxlcu.html

C#:   var value = data ?? "默认值";
来源：http://hz.daxiang520.top/gtphuqtgss.html

[A16] 真假值判断规则
来源：http://hz.zdqjudy.top/gtslufonui.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.zhengqikj.top/gtkglriaqw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sxryk.cn/gtfpjcmire.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.pycfn.com/gtmdkjatqs.html

TS:   if (!x) {}
来源：http://hz.jqgufenzy.top/gtpdewcrsb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.ydzc1.top/gtwgmzfsrk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.haohaochexian.top/gtqhuexofc.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.hnqzz.top/gttglwlick.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.pycfn.com/gtcxaitizw.html

[A17] 位运算
来源：http://hz.zhijiandao.cn/gteffwxjgg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtksucxhct.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ydzc1.top/gtsuitubsh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ivvv.top/gtigmstlta.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtpfycseko.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xinyue.icu/gtijivrigw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtwuiybsrb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtienxrexu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtdbnkeoun.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhoulong.xyz/gtdzerfimi.html

Py:   ord("A"); chr(65)
来源：http://hz.tian-w.cn/gtgdmfxvwb.html

PHP:  ord("A"); chr(65)
来源：http://hz.tanke756.top/gtneibojeu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinyuanbaomall.cn/gtkmvzxmam.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daxiang520.top/gtdkxttiwt.html

Java: (int) 'A'; (char) 65
来源：http://hz.jinyuanbaomall.cn/gtxnffmstz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.daxiang520.top/gtsiginagp.html

Ruby: "A".ord; 65.chr
来源：http://hz.fengsongda.top/gtljcprwyu.html

C#:   (int)'A'; (char)65
来源：http://hz.yonumen.top/gttiyhnyhj.html

[A19] 交换两个变量
来源：http://hz.bjfxy.top/gtangqqbxb.html

Py:   a, b = b, a
来源：http://hz.zycfv.cn/gthwuowprh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.gaohongyu789.top/gtgffamgfw.html

JS:   [a, b] = [b, a];
来源：http://hz.mhx1999.top/gtjcofkmvv.html

TS:   [a, b] = [b, a];
来源：http://hz.cucudq.cn/gtbcvgletw.html

Java: int t = a; a = b; b = t;
来源：http://hz.mhx1999.top/gtccfmcwsq.html

Go:   a, b = b, a
来源：http://hz.hywenlv.cn/gtyagktdst.html

Ruby: a, b = b, a
来源：http://hz.0kj1m.cn/gtecwtrlsc.html

C#:   (a, b) = (b, a);
来源：http://hz.wangdashe.top/gtpxybyvvb.html

[A20] 读取标准输入
来源：http://hz.jiagoushi.top/gtpvavhwrg.html

Py:   name = input("请输入：")
来源：http://hz.svipenyu.cn/gtncfuicww.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.sufxvd.cn/gthhyeykft.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jyoumei.cn/gtfldnvsio.html

TS:   // Node.js：readline 模块
来源：http://hz.gogol.net.cn/gtovmfwvmb.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.tanke756.top/gtmmljltez.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.snrcjt.cn/gtqsfayano.html

Ruby: gets.chomp
来源：http://hz.gotoacloud.top/gthsyvulaa.html

C#:   Console.ReadLine();
来源：http://hz.xylfe.cn/gtxsptrpsm.html

[A21] 保留指定小数位输出
来源：http://hz.haohaochexian.top/gtvmmenvwp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.wangshuangyany.cn/gtqwuzhlxn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cqqwz.cn/gtzklvjeht.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xziqi.cn/gtxwiidavm.html

TS:   (3.14159).toFixed(2)
来源：http://hz.feifeiyinyue.top/gtyoclkhws.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.nanxuanxn.top/gtlgepbftv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtadiuxizb.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.xuanzx.com/gtgmennktn.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj202588.top/gtbgudraxv.html

[A22] 获取字符串长度
来源：http://hz.xuetiantiany.cn/gtndedbwec.html

Py:   len(s)
来源：http://hz.daria6918.cn/gtjuzgrzyy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ydzc1.top/gtrwqnxjqb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhijiandao.cn/gtbblmlkcf.html

TS:   s.length
来源：http://hz.yvedp.cn/gthozeiwpn.html

Java: s.length()
来源：http://hz.yueranfly.top/gtzhfgoyqm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.snrcjt.cn/gtxfzcrrvi.html

Ruby: s.length
来源：http://hz.chenlongwang.top/gtroapwkic.html

C#:   s.Length
来源：http://hz.shanyushiyangkeji.top/gtrapjsmnk.html

[A23] 大小写转换
来源：http://hz.vqdsnc.cn/gtmdtntmoe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.pengpengdd.cyou/gtukcvqowd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xingfuxueyuan.xyz/gtbcswwdwf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.fzhhl.top/gtjadpsgop.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.guannengcc.top/gtynbmuhru.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.xylfe.cn/gtzwehuwnf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhaomingkeji.xyz/gtddbnjcbf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.fzhhl.top/gtwxtgsdec.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gaohongyu789.top/gtidzweepl.html

[A24] 去除首尾空白
来源：http://hz.tanke756.top/gtajeqvpre.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.nanxinkj.top/gtyxesckij.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.wangshuangyany.cn/gtrclruqge.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yvedp.cn/gtypimucve.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangshuangyany.cn/gttjzuvudq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ydzc1.top/gtkhardwjj.html

Go:   strings.TrimSpace(s)
来源：http://hz.nanxuanxn.top/gtifadavff.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zycfv.cn/gtiscwuacl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.havefunace.top/gtnljgruiv.html

[A25] 字符串比较
来源：http://hz.ivvv.top/gtcnongbnv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.quarkkingdee.top/gtvudxaceo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.pycfn.com/gtjrfcqmcy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.birdmap.top/gtwcuokyoi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.kuanghao11.cn/gtqyqqebil.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.andypj.xyz/gtqfavzfcw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cucudq.cn/gtynerxyzu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.bjfxy.top/gteajnxwrk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hnxiangtu.top/gteqoyvmsh.html

[A26] 类型转换总览
来源：http://hz.yongpay.top/gtwtribjvs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hammf.cn/gtptzdewwd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.c1oappe.top/gtrlufoljm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.9152youxi.cn/gtrqidqvyh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yongpay.top/gtdvymdzet.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jqgfzy.top/gtsbescsrx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.daria6918.cn/gtbqtnzwjh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.daxiang520.top/gtvcsqdgmr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.iojbl.cn/gtuevcjndk.html

================================================================================
来源：http://hz.cheryme.top/gtwgtmpxhh.html

B. 流程控制
来源：http://hz.xziqi.cn/gtppchmtue.html

================================================================================
来源：http://hz.daxiang520.top/gtketojllc.html

[B01] 条件判断 if / else
来源：http://hz.zhengqikj.top/gtjqsvysre.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zycfv.cn/gtaxvciwoo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cucudq.cn/gtkzowfuev.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nanxuanxn.top/gtqriqtdfa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtdsjfpevb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtkxtygpzk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.c1oappe.top/gtsnmnlnel.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.nwbrower.top/gtnboxnrfz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtxyuqpdze.html

[B02] 多分支 else if / elif
来源：http://hz.gotoacloud.top/gtjyabvxww.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xylfe.cn/gtuwkiwlgf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shangyingyoupin.top/gtsuqxbemq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.havefunace.top/gtgaroodvy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtooastvnq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtltjrcvnv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zdqjudy.top/gtdyemjiwt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ydzc1.top/gtjrfmuttq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.quarkkingdee.top/gtotzqbwme.html

[B03] switch / match / case
来源：http://hz.zycfv.cn/gtjrhuvccx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.0kj1m.cn/gtfnasusvs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hfpthk.cn/gtaywjkhfr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jianghu66.top/gtnkuixaas.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.meibo888.top/gtdyxjinpd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yangfankeji.com/gtwzpvsudg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.havefunace.top/gtraorcbtr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gtipyibtpp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cdnleiting.top/gtggudmjbc.html

[B04] for 计数循环
来源：http://hz.fengsongda.top/gtqulrdjzt.html

Py:   for i in range(10): print(i)
来源：http://hz.jqgfzy.top/gtsehrpqtw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ybcxt.top/gtlkryzqrh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtblqdotep.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shzxlz.cn/gtnygpeqrr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhongyouzk.top/gtiqjsedkh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cucudq.cn/gtxuzrneir.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xuanzx.com/gthoyqltxz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.mhx1999.top/gtzhvarpyo.html

[B05] 遍历数组 / 列表
来源：http://hz.zycfv.cn/gtetbfjddt.html

Py:   for item in arr: print(item)
来源：http://hz.sufxvd.cn/gtfkyhxrho.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gzhubu.top/gtipasbwtt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.sxryk.cn/gtmlhguuzr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ybcxt.top/gtyrrkgxfw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigfzy.top/gtkssnlvvo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cdnleiting.top/gtxxrrtqdi.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sufxvd.cn/gtpxixzswr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yanxiufei.cn/gtjcsrjkxa.html

[B06] 遍历字典 / 对象
来源：http://hz.feifeiyinyue.top/gtxzfpviuc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.redwolf501.top/gtdqualhbq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daxiang520.top/gtvavdgvid.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnxiangtu.top/gtquuiprlz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gtrvmkhgkf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.redwolf501.top/gtklzavlcj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.fzhhl.top/gtiitvwuyy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hongshengwenyu.top/gtjcnzxyni.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhiwuduotai.top/gttxxvugid.html

[B07] while 循环
来源：http://hz.daxiang520.top/gtyxazsxww.html

Py:   while i < 10: i += 1
来源：http://hz.jinyuanbaomall.cn/gtpvchkzgp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cheryme.top/gtyvxxghck.html

JS:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtndckispl.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtdgztwexr.html

Java: while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtfgqsmzkq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shuidangran.top/gtnwimrtrn.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cheryme.top/gtspzwfyru.html

C#:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtaftszysi.html

[B08] do-while（至少执行一次）
来源：http://hz.yonumen.top/gtfmdirtfc.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ywan-chungtsiang.top/gtbqwnefgv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.smart0.xyz/gtopayteoq.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtxxvlfcgf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gttfotqtwx.html

Java: do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtllejnomk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.wangshuangyany.cn/gtowshsbas.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yuxming.cn/gtvbcoeepb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gthimqptnn.html

[B09] break 与 continue
来源：http://hz.feifeiyinyue.top/gtxdtfvkqh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aibaodan.cn/gtjldskegx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zycfv.cn/gtrubfwpkc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gttwyehxtq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtqsjowygu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtztvkexsm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.vqdsnc.cn/gtcvbuksxe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenjidiqi.icu/gtycszcakp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtwortmvbk.html

[B10] 遍历同时拿索引
来源：http://hz.cheryme.top/gteuuoerpv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.mhx1999.top/gtexrzqvvj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sufxvd.cn/gtqcsvopty.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtseppgyss.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.52xcode.cn/gtbtggjpes.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ehwqpu.com/gtqosebitm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shangyingyoupin.top/gtxsoiulbd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xziqi.cn/gtfuroiufi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gaohongyu789.top/gttgimxrmm.html

[B11] 生成数字序列 / 区间
来源：http://hz.ydzc1.top/gtnlcuhxyz.html

Py:   list(range(0, 10, 2))
来源：http://hz.shangyingyoupin.top/gtkcxnmtdo.html

PHP:  range(0, 10, 2);
来源：http://hz.yuxming.cn/gtnfwcnjqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtldgludqf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gtuexzvddc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.iojbl.cn/gtkskuqgqf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gtlxqfiigr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinyuanbaomall.cn/gtxsofylwq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tianlin.xyz/gtcfrpfoup.html

[B12] 跳出多层循环
来源：http://hz.zhiwuduotai.top/gtqsysdohv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shangyingyoupin.top/gtameuvtyi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shangyingyoupin.top/gtkjlggvjn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cqqwz.cn/gtuoamixfg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtcahsdlsp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtndonlkpz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinqigufen.top/gtpnkuzaol.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhengqikj.top/gtwdpdwcwm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinyuanbaomall.cn/gtktduwwgx.html

[B13] 判断是否为数字
来源：http://hz.aibaodan.cn/gttihytfth.html

Py:   isinstance(x, (int, float))
来源：http://hz.sxryk.cn/gtjkppvrif.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtwyyhdfil.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.vqdsnc.cn/gtvftredlv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtqvqucyag.html

Java: x instanceof Number
来源：http://hz.zhaomingkeji.xyz/gtyaomamsh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.fengsongda.top/gtqstfexlu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhongyouzk.top/gthxnxsaar.html

C#:   x is int or double or decimal
来源：http://hz.nanxinkj.top/gtonjibycu.html

[B14] 判断值是否在集合内
来源：http://hz.vqdsnc.cn/gtnbrddout.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ydzc1.top/gtxvbeichd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aibaodan.cn/gtlbsvbmhz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtgjhcydjq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtnhrwlfii.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yvedp.cn/gtnpsgbqcr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sysykeji.top/gtvpqvnqoa.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yangfankeji.com/gttwyauybh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aizwys.cn/gtaobipkaj.html

[B15] 布尔运算与取反
来源：http://hz.yonumen.top/gtvnmsqrvo.html

Py:   a and b or not c
来源：http://hz.c1oappe.top/gtzocgfben.html

PHP:  $a && $b || !$c
来源：http://hz.yanxiufei.cn/gtsruwelpc.html

JS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtfxfzmjrk.html

TS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gteaoqmefr.html

Java: a && b || !c
来源：http://hz.yvedp.cn/gtmqwkpkng.html

Go:   a && b || !c
来源：http://hz.redwolf501.top/gtslzakiab.html

Ruby: a && b || !c
来源：http://hz.yj202588.top/gtptkpbrtb.html

C#:   a && b || !c
来源：http://hz.cqqwz.cn/gtocjbddnt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigfzy.top/gtukyzpsvu.html

Py:   if not data: return
来源：http://hz.pycfn.com/gtlxnrpdwu.html

PHP:  if (!$data) { return; }
来源：http://hz.daria6918.cn/gtzruwcklp.html

JS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtbfokbbdl.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtguloancx.html

Java: if (data == null) return;
来源：http://hz.c1oappe.top/gtnemgulzy.html

Go:   if data == nil { return }
来源：http://hz.sysykeji.top/gtvgqmtccg.html

Ruby: return if data.nil?
来源：http://hz.shzxlz.cn/gtivlpaivp.html

C#:   if (data == null) return;
来源：http://hz.9152youxi.cn/gtezkzmbvj.html

================================================================================
来源：http://hz.fengsongda.top/gttewsrjod.html

C. 函数与作用域
来源：http://hz.hywenlv.cn/gtmskoupsv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrdlhvtxs.html

[C01] 定义函数
来源：http://hz.xylfe.cn/gtptzuxcfu.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxinkj.top/gtaxshllvr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gttfjifuuy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ivvv.top/gtundmduuj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtbzswvzyi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtysxauynq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hywenlv.cn/gtnyogmjos.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangkeji.top/gtpwopcbch.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtunpdkbkf.html

[C02] 默认参数
来源：http://hz.sxryk.cn/gtbthdzjcz.html

Py:   def greet(name="World"): return name
来源：http://hz.wangshuangyany.cn/gtxhkqoyty.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtvlzpteil.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yvedp.cn/gteyiuiben.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yangfankeji.com/gtnmqojkdv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nwbrower.top/gtmlaawflx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhixingplan.top/gtmlaaakls.html

Ruby: def greet(name = "World") = name
来源：http://hz.dianchejie.cn/gtondthjtc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ehwqpu.com/gtssdzkdmr.html

[C03] 可变参数
来源：http://hz.dianchejie.cn/gteoarwbgj.html

Py:   def total(*args): return sum(args)
来源：http://hz.yvedp.cn/gteojbfzdp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jyoumei.cn/gtowpgsdxs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtfffzqmlj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gtxolfxpsi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtxquyijfw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuanzx.com/gtpczshssl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shuidangran.top/gtrbvpkuie.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhongyouzk.top/gtuisasogu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ivvv.top/gtkswhyvxv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cheryme.top/gtznfjlbfg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.snrcjt.cn/gtryixjydy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtcyzpqzbt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cucudq.cn/gtmkuhgthh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gtzjazzhdr.html


<!-- 参考信息 -->