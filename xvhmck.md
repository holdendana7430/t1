代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.sysykeji.top/gtamjpkwgx.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhongyouzk.top/gtxzwsqpdt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhiwuduotai.top/gtiyahkfwb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.guowangkeji.top/gtibtjoexz.html

Ruby: value = data || "默认值"
来源：http://hz.yj20258888.top/gtrhtcqcdw.html

C#:   var value = data ?? "默认值";
来源：http://hz.ydzc1.top/gtswrzlsgx.html

[A16] 真假值判断规则
来源：http://hz.yj202588.top/gtrxmzlqrw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.hnqzz.top/gtvfqikhkp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jqgufenzy.top/gtjfmwooaw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhongyouzk.top/gthsyagivw.html

TS:   if (!x) {}
来源：http://hz.jiagoushi.top/gttiswjsum.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shzxlz.cn/gthiwevvxr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.guannengcc.top/gtmfdgqhfn.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.aibaodan.cn/gtvncejmpw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.sysykeji.top/gtngbqifju.html

[A17] 位运算
来源：http://hz.yueranfly.top/gtucrxemay.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.birdmap.top/gtoxdckizk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.hnqzz.top/gtufgbhfok.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtxndororc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gtlzaiypcr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhaomingkeji.xyz/gtlnclswlg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gtymtwyglb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sysykeji.top/gtnznkrzeo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.svipenyu.cn/gtxabpenag.html

[A18] 字符与 ASCII 码互转
来源：http://hz.haohaochexian.top/gtalrtbgqw.html

Py:   ord("A"); chr(65)
来源：http://hz.jinghuilouyu.cn/gtlhrlstjz.html

PHP:  ord("A"); chr(65)
来源：http://hz.ywan-chungtsiang.top/gtsfkqxxwv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jyoumei.cn/gtauymamne.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yuxming.cn/gtyjexvfsf.html

Java: (int) 'A'; (char) 65
来源：http://hz.cqqwz.cn/gtgjdbadlz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.hnxiangtu.top/gttjtylvna.html

Ruby: "A".ord; 65.chr
来源：http://hz.9152youxi.cn/gtnvijyiow.html

C#:   (int)'A'; (char)65
来源：http://hz.yanxiufei.cn/gtkvtizylz.html

[A19] 交换两个变量
来源：http://hz.meibo888.top/gtampgzxia.html

Py:   a, b = b, a
来源：http://hz.chenjidiqi.icu/gtnprmzxjx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jinqigfzy.top/gttzytvfrm.html

JS:   [a, b] = [b, a];
来源：http://hz.yuxming.cn/gtvtcuswqk.html

TS:   [a, b] = [b, a];
来源：http://hz.jyoumei.cn/gtcuqfehvb.html

Java: int t = a; a = b; b = t;
来源：http://hz.mhx1999.top/gtemovymcp.html

Go:   a, b = b, a
来源：http://hz.snrcjt.cn/gtzvmvrfit.html

Ruby: a, b = b, a
来源：http://hz.birdmap.top/gtfshgidcp.html

C#:   (a, b) = (b, a);
来源：http://hz.cucudq.cn/gtupfujgki.html

[A20] 读取标准输入
来源：http://hz.jinghuilouyu.cn/gtibmivagn.html

Py:   name = input("请输入：")
来源：http://hz.cheryme.top/gtezyejjgj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.meibo888.top/gtzmehalba.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.bjfxy.top/gtvqhixzvj.html

TS:   // Node.js：readline 模块
来源：http://hz.gogol.net.cn/gtbpbuqzvc.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhoulong.xyz/gtkexieqlj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.c1oappe.top/gtnfdyqhrc.html

Ruby: gets.chomp
来源：http://hz.cqqwz.cn/gtocfblvrk.html

C#:   Console.ReadLine();
来源：http://hz.zdqjudy.top/gtvpqwxbah.html

[A21] 保留指定小数位输出
来源：http://hz.jinghuilouyu.cn/gtsudzjmhi.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yuanzhike.top/gttezjgiha.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhengqikj.top/gtjnlpexab.html

JS:   (3.14159).toFixed(2)
来源：http://hz.iojbl.cn/gtqhjtmnhb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.9152youxi.cn/gthhjazqew.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.svipenyu.cn/gtnpkacema.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.9152youxi.cn/gtfayqursh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yj20258888.top/gtlwharkbr.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj20258888.top/gthimsbyxd.html

[A22] 获取字符串长度
来源：http://hz.pengpengdd.cyou/gtliocdkvc.html

Py:   len(s)
来源：http://hz.nwbrower.top/gtfnbxoaop.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.aibaodan.cn/gtrlfegbtr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yvedp.cn/gtlggswcxf.html

TS:   s.length
来源：http://hz.gzhubu.top/gtqvrourny.html

Java: s.length()
来源：http://hz.guowangkeji.top/gtqqscrlbr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cucudq.cn/gtgcyhwyqc.html

Ruby: s.length
来源：http://hz.xinyue.icu/gtsqiigmnu.html

C#:   s.Length
来源：http://hz.vqdsnc.cn/gtadhrwvro.html

[A23] 大小写转换
来源：http://hz.shangyingyoupin.top/gtwcbmmoqd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.wangshuangyany.cn/gthppkaabu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xuetiantiany.cn/gtnaswcgrg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sysykeji.top/gtydgqwyoh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jiagoushi.top/gtywkpyiyr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yanxiufei.cn/gtbysgbbao.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.wangdashe.top/gtutfhzywj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ppjwa.cn/gtrugjzoxl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gotoacloud.top/gtloqjbvfy.html

[A24] 去除首尾空白
来源：http://hz.yongpay.top/gtokycitvj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yj20258.top/gtjmffzcax.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ybcxt.top/gtcqdnwbqy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ehwqpu.com/gtadffgdzi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sufxvd.cn/gtbyxvzkyr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.chenlongwang.top/gttkdfuiun.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhixingplan.top/gtrftgjeew.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yvedp.cn/gtubremqei.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.quarkkingdee.top/gtyaqnefrp.html

[A25] 字符串比较
来源：http://hz.yonumen.top/gtitsxifgc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.chenlongwang.top/gtugoiefca.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xinyue.icu/gthzxoscog.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.guowangkeji.top/gtzvduzdqm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xinyue.icu/gtckrzvjju.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jyoumei.cn/gtjecxbqwq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhoulong.xyz/gtjbrdydkz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hywenlv.cn/gtbuhqwdzs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daxiang520.top/gthezaqmsp.html

[A26] 类型转换总览
来源：http://hz.wangdashe.top/gtpmhokzmi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ydzc1.top/gtpezhcgvk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.nanxinkj.top/gtzdbbazeo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.quarkkingdee.top/gtgpnmzzxs.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zycfv.cn/gtodbqwpci.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jiagoushi.top/gthnsfozhf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sweek.top/gtblbgcrjv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.c1oappe.top/gtgtdktisi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.sxryk.cn/gtlhibszcf.html

================================================================================
来源：http://hz.yuanzhike.top/gtmeeehjfp.html

B. 流程控制
来源：http://hz.ybcxt.top/gtmvjovkyr.html

================================================================================
来源：http://hz.zycfv.cn/gtnklzebow.html

[B01] 条件判断 if / else
来源：http://hz.pengpengdd.cyou/gtmwapahaz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zycfv.cn/gthmfkfhjg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jinyuanbaomall.cn/gtgrwxfejm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtkvfrqglo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gtvzwnhkyk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtpctyjuym.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hywenlv.cn/gtveltpgbw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.daria6918.cn/gtibfmretm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gtnfcaclzw.html

[B02] 多分支 else if / elif
来源：http://hz.jinyuanbaomall.cn/gtfvxtdzeh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhongyouzk.top/gtrdiqjyzs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shanyushiyangkeji.top/gtpemnyjxo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtjfendkru.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtshlopouv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gthteakexf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.pycfn.com/gtubnxtpbx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.tanke756.top/gtsofssktl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtlgmpjbjm.html

[B03] switch / match / case
来源：http://hz.jlsjyb.cn/gtivjkorcb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jiagoushi.top/gtdbjcqbwl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jlsjyb.cn/gtunglygfe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zycfv.cn/gthdlapvwz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xuanzx.com/gtunawswwg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.haohaochexian.top/gttsxqqiod.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ivvv.top/gtiwnnhqjy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cqqwz.cn/gtsnyhmvct.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ppjwa.cn/gtrkifeoid.html

[B04] for 计数循环
来源：http://hz.xuanzx.com/gtqrihnuaa.html

Py:   for i in range(10): print(i)
来源：http://hz.jinqigfzy.top/gtbnrkmjxq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ywan-chungtsiang.top/gtesqnczgf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zycfv.cn/gtdrsnoulc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yonumen.top/gtbjjmalwm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ehwqpu.com/gtwxunwxto.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinqigfzy.top/gtqtwgnyrn.html

Ruby: 10.times { |i| puts i }
来源：http://hz.wangdashe.top/gtsjacmmzw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.andypj.xyz/gtmspnhqiu.html

[B05] 遍历数组 / 列表
来源：http://hz.andypj.xyz/gtrwbjuoqv.html

Py:   for item in arr: print(item)
来源：http://hz.zhoulong.xyz/gtiafsaubj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.redwolf501.top/gtcxoflxot.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.gzhubu.top/gthwrvuwsv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hysaishi.cn/gtgvuzscei.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jyoumei.cn/gtfxfhrcyx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jqgufenzy.top/gtotlvzyvu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhengqikj.top/gtmuvdleci.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gaohongyu789.top/gteafvgsdp.html

[B06] 遍历字典 / 对象
来源：http://hz.yangfankeji.com/gtqwgqsbvr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.tian-w.cn/gtcldgyvsq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.havefunace.top/gtsfktiywa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cqqwz.cn/gtvnrzrydi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cheryme.top/gtfnhyrech.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sxryk.cn/gtrqgvmlvy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.tian-w.cn/gtzibfomqu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hywenlv.cn/gtiyqjzpvr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shanyushiyangtech.top/gtlifegqnu.html

[B07] while 循环
来源：http://hz.sufxvd.cn/gtbthhzyjr.html

Py:   while i < 10: i += 1
来源：http://hz.gogol.net.cn/gtpdburexi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.shuidangran.top/gtkngdozvw.html

JS:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtddhaolxc.html

TS:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtfybqrtpc.html

Java: while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtdovqcuaf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sysykeji.top/gtuhljbpao.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nanxuanxn.top/gtnoqinesf.html

C#:   while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtfajudxur.html

[B08] do-while（至少执行一次）
来源：http://hz.sysykeji.top/gtolzrxwka.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shanyushiyangkeji.top/gtyaywympm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jinghuilouyu.cn/gtoinehlvu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtkqpwqmzp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtbtvfkbys.html

Java: do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtsybuavzp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhengqikj.top/gtrcmmqlvr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.daria6918.cn/gtvkrodwvv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtvtykzdwl.html

[B09] break 与 continue
来源：http://hz.jyoumei.cn/gtiiejumjz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xylfe.cn/gthtrajmal.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.smart0.xyz/gtnjlqhkxb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtvvmtiwky.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtkozdcqtp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtujhbqlsd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nanxinkj.top/gtzkrmjgzn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sxryk.cn/gtzklrkcvh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gtwkibawee.html

[B10] 遍历同时拿索引
来源：http://hz.yueranfly.top/gtvlwwxkix.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gzhubu.top/gtlebtjrek.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cashguo.top/gtmrwameah.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtrywngsrv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhiwuduotai.top/gtdjhhajoz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.0kj1m.cn/gturywndrv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ywan-chungtsiang.top/gtpktptlax.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aibaodan.cn/gtpazahyml.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtjbcagyak.html

[B11] 生成数字序列 / 区间
来源：http://hz.yvedp.cn/gtxabobksw.html

Py:   list(range(0, 10, 2))
来源：http://hz.sufxvd.cn/gtubtmccmd.html

PHP:  range(0, 10, 2);
来源：http://hz.cucudq.cn/gtwgvnbxlq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtiwfatpwn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pengpengdd.cyou/gtajicakrj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shangyingyoupin.top/gtsotbknnu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yueranfly.top/gtywjsqevr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ywan-chungtsiang.top/gtivvjkefh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.bjfxy.top/gtyyxdbyse.html

[B12] 跳出多层循环
来源：http://hz.jqgfzy.top/gtqanjrtsz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.wangdashe.top/gtqglelwtj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinqigufen.top/gtortxyddt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtwjdpvcru.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtyhltochu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtviwxhnok.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtpojqbhmz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fzhhl.top/gtsjpfjaum.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhengqikj.top/gtstoidfvh.html

[B13] 判断是否为数字
来源：http://hz.c1oappe.top/gttqjnrblp.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigfzy.top/gtukrrowjn.html

PHP:  is_numeric($x)
来源：http://hz.sufxvd.cn/gthyapeytp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtnbikvcin.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtwlcexgmf.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gtnddcwyvt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.0kj1m.cn/gtmakhwizg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ydjk.org.cn/gtxkwsvzen.html

C#:   x is int or double or decimal
来源：http://hz.tanke756.top/gtajmfnyeq.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtbqrjmfgk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.redwolf501.top/gtoumzrrkd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cheryme.top/gtjpggmqwt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sysykeji.top/gtmvzyybek.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtcfeiliev.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.daxiang520.top/gtljhqiuru.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yuanzhike.top/gtgwqxkleh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.vqdsnc.cn/gtliqmmcql.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj202588.top/gtvynzkplr.html

[B15] 布尔运算与取反
来源：http://hz.sxryk.cn/gtxhunnjii.html

Py:   a and b or not c
来源：http://hz.zhaomingkeji.xyz/gtflptjsgx.html

PHP:  $a && $b || !$c
来源：http://hz.yj202588.top/gtmxwqebei.html

JS:   a && b || !c
来源：http://hz.daxiang520.top/gtgpspzrzj.html

TS:   a && b || !c
来源：http://hz.fengsongda.top/gtmmgsgfnj.html

Java: a && b || !c
来源：http://hz.yvedp.cn/gtzqsnzhlk.html

Go:   a && b || !c
来源：http://hz.pycfn.com/gtdjgnyggg.html

Ruby: a && b || !c
来源：http://hz.jinqigfzy.top/gtkqwrwphf.html

C#:   a && b || !c
来源：http://hz.c1oappe.top/gtvsgqwecr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sysykeji.top/gtujrjriyq.html

Py:   if not data: return
来源：http://hz.316326.xyz/gtgjfxcnxy.html

PHP:  if (!$data) { return; }
来源：http://hz.yuanzhike.top/gtczkpmlrm.html

JS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtxvuteocq.html

TS:   if (!data) return;
来源：http://hz.sysykeji.top/gtwtrcrmpn.html

Java: if (data == null) return;
来源：http://hz.xinyue.icu/gtuhnmcvjd.html

Go:   if data == nil { return }
来源：http://hz.aizwys.cn/gtyjjcmpio.html

Ruby: return if data.nil?
来源：http://hz.chenlongwang.top/gtypshgylz.html

C#:   if (data == null) return;
来源：http://hz.cashguo.top/gtfbthetbf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtktjavvos.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtmraemiho.html

================================================================================
来源：http://hz.shzxlz.cn/gtopzjihgt.html

[C01] 定义函数
来源：http://hz.zhixingplan.top/gtphdbrpvc.html

Py:   def add(a, b): return a + b
来源：http://hz.guannengcc.top/gtungcsuxi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtdjeoklcj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cucudq.cn/gtlvodahum.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtvxryzbur.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtrrlsysju.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.redwolf501.top/gtjervkbxz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenlongwang.top/gtwgdvodxc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtxztsvogd.html

[C02] 默认参数
来源：http://hz.cdnleiting.top/gtshxkjlci.html

Py:   def greet(name="World"): return name
来源：http://hz.zhiwuduotai.top/gtyfkihohl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hysaishi.cn/gtgrnsohwz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gtbfdjezrt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhoulong.xyz/gtobfheeuh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhongyouzk.top/gtoclsdhdh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.iojbl.cn/gtbdvxlicb.html

Ruby: def greet(name = "World") = name
来源：http://hz.bjfxy.top/gtzcpmkuil.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gtdhjznmzu.html

[C03] 可变参数
来源：http://hz.shanyushiyangtech.top/gtrehlalwu.html

Py:   def total(*args): return sum(args)
来源：http://hz.ywan-chungtsiang.top/gtjjpzlskc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhongyouzk.top/gtlbpkjscj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gogol.net.cn/gtguzoijds.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtkfulpygs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.52xcode.cn/gttklxvqes.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.c1oappe.top/gtpnzcbvwh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hongshengwenyu.top/gtwdvoqori.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cucudq.cn/gtqvopwall.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sufxvd.cn/gttlgyxdse.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.andypj.xyz/gtmlezsusu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigufen.top/gtuearjkoo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtmrcbbain.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtlxnjjdfh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sysykeji.top/gtcndqnkla.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtjeyphpph.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zycfv.cn/gtopnimuzm.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtwelvlxed.html

[C05] 返回多个值
来源：http://hz.meibo888.top/gtbrdolirj.html

Py:   return a, b
来源：http://hz.shzxlz.cn/gtqvpyzlej.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtpatpolao.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.haohaochexian.top/gtvgfhbwai.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gtncrhgatv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtjeafeibk.html

Go:   return a, b
来源：http://hz.nwbrower.top/gthncuplau.html

Ruby: return a, b
来源：http://hz.kuanghao11.cn/gtkawkjiaw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gzhubu.top/gtomiwdpgx.html


<!-- 参考信息 -->