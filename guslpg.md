代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.0kj1m.cn/gtccwvcbtr.html

Go:   "第一行\n第二行"
来源：http://hz.guowangkeji.top/gtilektmll.html

Ruby: "第一行\n第二行"
来源：http://hz.daria6918.cn/gthgntwejt.html

C#:   "第一行\n第二行"
来源：http://hz.sysykeji.top/gtjbwjmrhz.html

[A14] 注释写法
来源：http://hz.sxryk.cn/gtnklihqon.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.52xcode.cn/gthhgrqxtb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.aibaodan.cn/gtezsyouwp.html

JS:   // 单行；/* 多行 */
来源：http://hz.chenlongwang.top/gtrecfojzs.html

TS:   // 单行；/* 多行 */
来源：http://hz.yueranfly.top/gtesktejlg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jinqigufen.top/gtljvmgyyd.html

Go:   // 单行；/* 多行 */
来源：http://hz.zhoulong.xyz/gtfkbsouek.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.xuetiantiany.cn/gthzbcivlx.html

C#:   // 单行；/* 多行 */
来源：http://hz.guannengcc.top/gtscarfhip.html

[A15] 空值判断与默认值
来源：http://hz.aibaodan.cn/gtcjolbbhq.html

Py:   value = data or "默认值"
来源：http://hz.ydjk.org.cn/gttljwmjpo.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.tian-w.cn/gtqfxzpclb.html

JS:   const value = data ?? "默认值";
来源：http://hz.sweek.top/gtfgguxujw.html

TS:   const value = data ?? "默认值";
来源：http://hz.0kj1m.cn/gtxzwufjdf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.ehwqpu.com/gtorjkqvli.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.gotoacloud.top/gtyfqomajr.html

Ruby: value = data || "默认值"
来源：http://hz.xuetiantiany.cn/gtlqzavvxo.html

C#:   var value = data ?? "默认值";
来源：http://hz.chenzaomai.com/gtcalxbnkx.html

[A16] 真假值判断规则
来源：http://hz.hywenlv.cn/gtwrfvprpw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ehwqpu.com/gtximzrnlu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.316326.xyz/gtiymkrzgy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.nanxuanxn.top/gtvbnhnbpn.html

TS:   if (!x) {}
来源：http://hz.aibaodan.cn/gtdgpmuljv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hnqzz.top/gtgzapdfcr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.hongshengwenyu.top/gtuspcddkm.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.shangyingyoupin.top/gtzifbvnbx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hywenlv.cn/gtelcaunur.html

[A17] 位运算
来源：http://hz.nanxinkj.top/gtzdbevhkk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jqgfzy.top/gtlwdobvxt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.shzxlz.cn/gtqqxiysfy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtngvxzrkp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtouigvpai.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtcmxzofou.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gtcpavjdtd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gtccfstcso.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yonumen.top/gtqealofmj.html

[A18] 字符与 ASCII 码互转
来源：http://hz.tian-w.cn/gtynlkdjms.html

Py:   ord("A"); chr(65)
来源：http://hz.zhijiandao.cn/gtvhcmzppe.html

PHP:  ord("A"); chr(65)
来源：http://hz.52xcode.cn/gtpciamskc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.fzhhl.top/gtjfuxxgvm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yj202588.top/gtoubdxaqc.html

Java: (int) 'A'; (char) 65
来源：http://hz.chenjidiqi.icu/gtvexdbmlt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.mhx1999.top/gtquatbaey.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhijiandao.cn/gtpmgjsdug.html

C#:   (int)'A'; (char)65
来源：http://hz.kuanghao11.cn/gtlzskpmtw.html

[A19] 交换两个变量
来源：http://hz.zhongyouzk.top/gtfbirlhcc.html

Py:   a, b = b, a
来源：http://hz.gotoacloud.top/gtfwwzkdcy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shzxlz.cn/gtizshsnub.html

JS:   [a, b] = [b, a];
来源：http://hz.guannengcc.top/gtvepxamqs.html

TS:   [a, b] = [b, a];
来源：http://hz.sxryk.cn/gtajppeiun.html

Java: int t = a; a = b; b = t;
来源：http://hz.daxiang520.top/gtwhazmuxc.html

Go:   a, b = b, a
来源：http://hz.cqqwz.cn/gthmcexpag.html

Ruby: a, b = b, a
来源：http://hz.nwbrower.top/gtaicrxcdt.html

C#:   (a, b) = (b, a);
来源：http://hz.hysaishi.cn/gtkxfattep.html

[A20] 读取标准输入
来源：http://hz.yuanzhike.top/gtdzygtxkw.html

Py:   name = input("请输入：")
来源：http://hz.ivvv.top/gtwwzqehtl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.aizwys.cn/gtbeodttkh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.aibaodan.cn/gtvnlawmwv.html

TS:   // Node.js：readline 模块
来源：http://hz.jinqigufen.top/gtyljaicgx.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhengqikj.top/gtlthhqxyl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yj202588.top/gtpxvhplui.html

Ruby: gets.chomp
来源：http://hz.hysaishi.cn/gtllugsbco.html

C#:   Console.ReadLine();
来源：http://hz.feifeiyinyue.top/gtchnuxdyn.html

[A21] 保留指定小数位输出
来源：http://hz.daxiang520.top/gtfwiyllwr.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jiagoushi.top/gturemwrek.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yj20258.top/gtcyimpfkk.html

JS:   (3.14159).toFixed(2)
来源：http://hz.nanxinkj.top/gtrmjfsnnp.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sweek.top/gtjphoxmxt.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtatdvbqym.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtpcmvwihv.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.cdnleiting.top/gtugbhklts.html

C#:   3.14159.ToString("F2")
来源：http://hz.sufxvd.cn/gtrabkrmlj.html

[A22] 获取字符串长度
来源：http://hz.cdnleiting.top/gtlhnnqopd.html

Py:   len(s)
来源：http://hz.tanke756.top/gtxgcnpxrl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.smart0.xyz/gtllcjxvxg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.pengpengdd.cyou/gtiyknbcxu.html

TS:   s.length
来源：http://hz.zhixingplan.top/gtyxkqnkxl.html

Java: s.length()
来源：http://hz.fzhhl.top/gtumtjgbut.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zycfv.cn/gtecjlrnyb.html

Ruby: s.length
来源：http://hz.wangshuangyany.cn/gtmxorvuew.html

C#:   s.Length
来源：http://hz.shuidangran.top/gtrtxijrme.html

[A23] 大小写转换
来源：http://hz.jyoumei.cn/gtxwcnfdiz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.kuanghao11.cn/gtuhnbryru.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zdqjudy.top/gttcqklyrl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtnmwdbgmg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ppjwa.cn/gttyfsroge.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxinkj.top/gtrvuoelgi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhiwuduotai.top/gtosqzppdm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jqgfzy.top/gtzsytxzsq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jiagoushi.top/gtkshyppld.html

[A24] 去除首尾空白
来源：http://hz.aizwys.cn/gtlnmtniyz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hnxiangtu.top/gtnlocljtb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.0kj1m.cn/gtxsmrlzzi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhijiandao.cn/gtadizcfmt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sysykeji.top/gtbvpwilyc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zhengqikj.top/gtdsdfgwik.html

Go:   strings.TrimSpace(s)
来源：http://hz.hnqzz.top/gtmtashdon.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.bjfxy.top/gtggtbirdj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shzxlz.cn/gtpwddjqmn.html

[A25] 字符串比较
来源：http://hz.bjfxy.top/gtjteplodk.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cdnleiting.top/gtuzyerldg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.redwolf501.top/gthsonmjxu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.feifeiyinyue.top/gtnvbkzfdx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtvizqleag.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.cashguo.top/gtzibiwpmu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zdqjudy.top/gtiesfniyh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.vqdsnc.cn/gtaynteyab.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xinyue.icu/gtglboaowm.html

[A26] 类型转换总览
来源：http://hz.wangdashe.top/gtdgqberey.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.haohaochexian.top/gtxkjdybtt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jiagoushi.top/gtlfynpsif.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yj202588.top/gtntgohuxn.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shzxlz.cn/gtuvhzpgnq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jlsjyb.cn/gtqlztuopf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jlsjyb.cn/gtepmildfh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shangyingyoupin.top/gtusfwurdo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.316326.xyz/gttgaxjubj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrvixrshw.html

B. 流程控制
来源：http://hz.ybcxt.top/gtpnpgdsak.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwonxlbyj.html

[B01] 条件判断 if / else
来源：http://hz.fengsongda.top/gtzqxalxkd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cheryme.top/gtfgbuzdiz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.dianchejie.cn/gttoetqhtu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yvedp.cn/gtoxrhpdbw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gtfpiddfzk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.tanke756.top/gtvvxiftpt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yueranfly.top/gtebluyobz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yvedp.cn/gtgpvclnfv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xingfuxueyuan.xyz/gtorrkupaj.html

[B02] 多分支 else if / elif
来源：http://hz.dashuyun.cn/gtwybetamt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yongpay.top/gtpyleuvvh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.pengpengdd.cyou/gtklyllbxn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtawkjutca.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnqzz.top/gtnsmjuaeh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinyuanbaomall.cn/gtwwreilom.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.haohaochexian.top/gtaxdbzlis.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinyuanbaomall.cn/gtvvrgtohj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangkeji.top/gtihlogvch.html

[B03] switch / match / case
来源：http://hz.hnxiangtu.top/gtlyxxsqnl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.0kj1m.cn/gtbpxftzmp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtnvdxxfoo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhengqikj.top/gthstqreff.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.52xcode.cn/gtxzcovmxo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shzxlz.cn/gtpqilzvpl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yanxiufei.cn/gtbpdltbxf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ppjwa.cn/gtxejmosjm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.dianchejie.cn/gtbmdnufrv.html

[B04] for 计数循环
来源：http://hz.0kj1m.cn/gtxbyfesyi.html

Py:   for i in range(10): print(i)
来源：http://hz.zycfv.cn/gthoiddodk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.tanke756.top/gtxsvcjivw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xylfe.cn/gtjkccxhmf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cdnleiting.top/gttvjghzjk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.gotoacloud.top/gtwtinmgxe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jiagoushi.top/gtycolhjjm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xziqi.cn/gtjbpisiuc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.nanxinkj.top/gtkowztima.html

[B05] 遍历数组 / 列表
来源：http://hz.jqgfzy.top/gtfxdpwsvu.html

Py:   for item in arr: print(item)
来源：http://hz.cqqwz.cn/gthsnkyanc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cqqwz.cn/gtqzfknkdd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yvedp.cn/gtxkluogac.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhongyouzk.top/gtgtnzihvv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.iojbl.cn/gtndvdrwlu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gogol.net.cn/gtntgddywr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jiagoushi.top/gtlpxodape.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ydzc1.top/gthylycvec.html

[B06] 遍历字典 / 对象
来源：http://hz.xylfe.cn/gthbwjgmnb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jiagoushi.top/gtjehiteng.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shangyingyoupin.top/gthwcgzbzc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.smart0.xyz/gtxecvzsrn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtklnfymnn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hywenlv.cn/gtsqizmhdi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sweek.top/gtalmhzayo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.kuanghao11.cn/gtvvyekrlp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.chenjidiqi.icu/gtimgfrcpp.html

[B07] while 循环
来源：http://hz.aizwys.cn/gtydisftwo.html

Py:   while i < 10: i += 1
来源：http://hz.hammf.cn/gtmqjhbiko.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.tianlin.xyz/gtcqxldftx.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtjtwmeind.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhengqikj.top/gtisrkqzqj.html

Java: while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gttowtcfub.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xingfuxueyuan.xyz/gtpsnshlmg.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ppjwa.cn/gtfbdcacwr.html

C#:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtcadygoxy.html

[B08] do-while（至少执行一次）
来源：http://hz.hysaishi.cn/gtezjcjeac.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.haohaochexian.top/gtcxysjcrd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.svipenyu.cn/gteftmjebu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtklsjjfdu.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtfuuolnzy.html

Java: do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtiuchiong.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shangyingyoupin.top/gtiujihcqf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinqigfzy.top/gtcxfpmrxa.html

C#:   do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtppbanndq.html

[B09] break 与 continue
来源：http://hz.gaohongyu789.top/gtsfnkbvyu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xziqi.cn/gticopbomy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtoecydtzs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gtrsnnsozm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gttzwcrwot.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtzywednlj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenjidiqi.icu/gtaddjwpyw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shanyushiyangkeji.top/gtcsqazvpw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtoilwujjf.html

[B10] 遍历同时拿索引
来源：http://hz.guannengcc.top/gtqeflsolr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtfthngsfr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinyuanbaomall.cn/gtqpewipez.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fengsongda.top/gtcapanacp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sufxvd.cn/gtukzvivby.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhongyouzk.top/gtutmkcnqx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hnqzz.top/gtyqtpwidi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhengqikj.top/gtullunwky.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yonumen.top/gtsrbtdtaw.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinyuanbaomall.cn/gtrcujegzk.html

Py:   list(range(0, 10, 2))
来源：http://hz.cqqwz.cn/gtqbjevvan.html

PHP:  range(0, 10, 2);
来源：http://hz.redwolf501.top/gtiqprcfyo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtzgmjrxrh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinyuanbaomall.cn/gtwwtmfltr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhoulong.xyz/gtnrfnyybb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhiwuduotai.top/gtfcljemqu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtcifxupsi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhijiandao.cn/gtexkqkhlt.html

[B12] 跳出多层循环
来源：http://hz.yangfankeji.com/gtvinhsdcs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jlsjyb.cn/gthhyzszer.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ydzc1.top/gtvenhoobf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangkeji.top/gtfxriwalc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtvpgqgaei.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtswjslmno.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ywan-chungtsiang.top/gtxocnrndp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gogol.net.cn/gtqthrbvuv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sweek.top/gtsizitfxl.html

[B13] 判断是否为数字
来源：http://hz.tianlin.xyz/gtrnggmqam.html

Py:   isinstance(x, (int, float))
来源：http://hz.cheryme.top/gtwcaieybf.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtyyedwmyq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gthshojuml.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gttjgwammo.html

Java: x instanceof Number
来源：http://hz.nanxinkj.top/gtwrsbldqa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daxiang520.top/gtbtasiigv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.havefunace.top/gtrrdbpvfv.html

C#:   x is int or double or decimal
来源：http://hz.dianchejie.cn/gtbgfqppdp.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtrdpxzxwd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.pengpengdd.cyou/gtjbsoojmr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgfzy.top/gtfvlxkiua.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tian-w.cn/gtepklmalp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sysykeji.top/gtkhynhlye.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.redwolf501.top/gtyrbodaiv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.snrcjt.cn/gteiyimkej.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sxryk.cn/gtpgxrzaad.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yvedp.cn/gtyhyadrbu.html

[B15] 布尔运算与取反
来源：http://hz.xinyue.icu/gtgldjnvck.html

Py:   a and b or not c
来源：http://hz.chenzaomai.com/gtjeuqcbkk.html

PHP:  $a && $b || !$c
来源：http://hz.zhijiandao.cn/gtvzvooftb.html

JS:   a && b || !c
来源：http://hz.yonumen.top/gtfaotppyy.html

TS:   a && b || !c
来源：http://hz.iojbl.cn/gtpqnvqlqv.html

Java: a && b || !c
来源：http://hz.yj20258888.top/gtcefjsqsx.html

Go:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtvnesmcuz.html

Ruby: a && b || !c
来源：http://hz.ydzc1.top/gtunlmvotj.html

C#:   a && b || !c
来源：http://hz.daxiang520.top/gthjivdtqb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ybcxt.top/gtwzaotxqb.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gtfdibbyac.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtzkltezmh.html

JS:   if (!data) return;
来源：http://hz.guannengcc.top/gtfekqcovm.html

TS:   if (!data) return;
来源：http://hz.yuanzhike.top/gtxccvwdvf.html

Java: if (data == null) return;
来源：http://hz.zdqjudy.top/gtoadkepmf.html

Go:   if data == nil { return }
来源：http://hz.yj202588.top/gtbpractdx.html

Ruby: return if data.nil?
来源：http://hz.jinqigufen.top/gtbhdasomv.html

C#:   if (data == null) return;
来源：http://hz.tanke756.top/gtfgfxeoxa.html

================================================================================
来源：http://hz.vqdsnc.cn/gtezhacfsf.html

C. 函数与作用域
来源：http://hz.zhaomingkeji.xyz/gtgtsotdnh.html

================================================================================
来源：http://hz.xinyue.icu/gtlyiqiikt.html

[C01] 定义函数
来源：http://hz.c1oappe.top/gtxpuvzqpf.html

Py:   def add(a, b): return a + b
来源：http://hz.zhengqikj.top/gtrovfhepg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtaqcjgwqm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtgmajkzsl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtminsqmfh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtdlvpemsu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtoetpwaha.html

Ruby: def add(a, b); a + b; end
来源：http://hz.birdmap.top/gtjdhtkjvb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtrxlmcwaj.html

[C02] 默认参数
来源：http://hz.yj20258.top/gtskfwqcxp.html

Py:   def greet(name="World"): return name
来源：http://hz.316326.xyz/gtgzlkzxcz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.birdmap.top/gtpixxnnec.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.kuanghao11.cn/gtushspnpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hammf.cn/gttifztszc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xinyue.icu/gtzphqbmrx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ydjk.org.cn/gtysvehlpj.html

Ruby: def greet(name = "World") = name
来源：http://hz.vqdsnc.cn/gtifkpgyrs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigufen.top/gtnyhhlzee.html

[C03] 可变参数
来源：http://hz.zhixingplan.top/gtzbghbpoj.html

Py:   def total(*args): return sum(args)
来源：http://hz.c1oappe.top/gtogxjczbi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yuanzhike.top/gtpqyphaql.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yongpay.top/gtgismxpts.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtotcunlmt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtlsstgalu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gzhubu.top/gtkqcnncfu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuetiantiany.cn/gtmbysebqp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtzxyuaubt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xingfuxueyuan.xyz/gtpqxxsnan.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.feifeiyinyue.top/gtwpyqicjm.html


<!-- 参考信息 -->