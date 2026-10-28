代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.nwbrower.top/gtsnodampy.html

Go:   "第一行\n第二行"
来源：http://hz.birdmap.top/gtqrgwrbrr.html

Ruby: "第一行\n第二行"
来源：http://hz.xylfe.cn/gtglidxgmj.html

C#:   "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtnnhylujv.html

[A14] 注释写法
来源：http://hz.smart0.xyz/gtvbdkbdtt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhiwuduotai.top/gtathcoyon.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.shuidangran.top/gtzeqxcxln.html

JS:   // 单行；/* 多行 */
来源：http://hz.yuanzhike.top/gtvaeqoqnd.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhengqikj.top/gtgkzpaxta.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.ydzc1.top/gtpsxxxeld.html

Go:   // 单行；/* 多行 */
来源：http://hz.birdmap.top/gtcakbnaxp.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.kuanghao11.cn/gtftuttxil.html

C#:   // 单行；/* 多行 */
来源：http://hz.9152youxi.cn/gtcpduizof.html

[A15] 空值判断与默认值
来源：http://hz.jinghuilouyu.cn/gtjgeepacu.html

Py:   value = data or "默认值"
来源：http://hz.guannengcc.top/gtevlfndvy.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.sysykeji.top/gtwylrbuqo.html

JS:   const value = data ?? "默认值";
来源：http://hz.jinqigufen.top/gtraibxtkc.html

TS:   const value = data ?? "默认值";
来源：http://hz.jinghuilouyu.cn/gthucaofqm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.aizwys.cn/gtmijrwpnu.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.feifeiyinyue.top/gtexlqtasg.html

Ruby: value = data || "默认值"
来源：http://hz.jyoumei.cn/gtfygekrsg.html

C#:   var value = data ?? "默认值";
来源：http://hz.daria6918.cn/gtoosmqizl.html

[A16] 真假值判断规则
来源：http://hz.guannengcc.top/gtqnfnbqyx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.svipenyu.cn/gtzwvjmjmk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.pengpengdd.cyou/gtjfwtkdjk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jinghuilouyu.cn/gtafpucghl.html

TS:   if (!x) {}
来源：http://hz.yangfankeji.com/gtxwxbxncn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yonumen.top/gtvtswvqsk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zdqjudy.top/gtzfphepon.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ywan-chungtsiang.top/gtzpcgoqop.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zhaomingkeji.xyz/gtcswfqkpw.html

[A17] 位运算
来源：http://hz.hnxiangtu.top/gtaaoxhauk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sysykeji.top/gtlfcfhkht.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.c1oappe.top/gtdxhjuvvf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.quarkkingdee.top/gtrpmacjqs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.gogol.net.cn/gtnqffkdkx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtedmtglce.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.andypj.xyz/gtfjiwbrje.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhongyouzk.top/gtvtfzrfay.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hywenlv.cn/gthsxaqjhu.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ydzc1.top/gtwviacuog.html

Py:   ord("A"); chr(65)
来源：http://hz.cucudq.cn/gtcuvszckm.html

PHP:  ord("A"); chr(65)
来源：http://hz.jyoumei.cn/gtaputeywx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yanxiufei.cn/gtjdwgciix.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yuxming.cn/gtqfmvtmpq.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhiwuduotai.top/gtlgbeefea.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.aibaodan.cn/gtotrevcfq.html

Ruby: "A".ord; 65.chr
来源：http://hz.daria6918.cn/gtsatkjzsz.html

C#:   (int)'A'; (char)65
来源：http://hz.gzhubu.top/gtjhkqogzk.html

[A19] 交换两个变量
来源：http://hz.zycfv.cn/gtfuzwqhtd.html

Py:   a, b = b, a
来源：http://hz.nwbrower.top/gtzgdowkzu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shangyingyoupin.top/gtwkyqwuwh.html

JS:   [a, b] = [b, a];
来源：http://hz.aibaodan.cn/gtoiiqmsim.html

TS:   [a, b] = [b, a];
来源：http://hz.feifeiyinyue.top/gtzmideclc.html

Java: int t = a; a = b; b = t;
来源：http://hz.fzhhl.top/gtpdinzgoq.html

Go:   a, b = b, a
来源：http://hz.gotoacloud.top/gtjohgivjl.html

Ruby: a, b = b, a
来源：http://hz.cashguo.top/gtaqhlzmgc.html

C#:   (a, b) = (b, a);
来源：http://hz.chenjidiqi.icu/gtldnxeytc.html

[A20] 读取标准输入
来源：http://hz.xziqi.cn/gtyrhvmspj.html

Py:   name = input("请输入：")
来源：http://hz.jiagoushi.top/gtqjqilstd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yuanzhike.top/gtnqodamph.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xuetiantiany.cn/gtnzeiuiad.html

TS:   // Node.js：readline 模块
来源：http://hz.sufxvd.cn/gtfxeddpnq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yonumen.top/gtgtrwmfbg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.shanyushiyangtech.top/gtdohdbkis.html

Ruby: gets.chomp
来源：http://hz.nanxuanxn.top/gtslckpkmg.html

C#:   Console.ReadLine();
来源：http://hz.cheryme.top/gtgpykxgbb.html

[A21] 保留指定小数位输出
来源：http://hz.shangyingyoupin.top/gtezxexlfy.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zdqjudy.top/gtxzhkvtqv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.nwbrower.top/gtkrejpoiu.html

JS:   (3.14159).toFixed(2)
来源：http://hz.meibo888.top/gtmhlsdvgw.html

TS:   (3.14159).toFixed(2)
来源：http://hz.gzhubu.top/gtsbjksngd.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtxwiwolmp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtcrxzktyf.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ydjk.org.cn/gtqawqfcno.html

C#:   3.14159.ToString("F2")
来源：http://hz.cucudq.cn/gthiryduxm.html

[A22] 获取字符串长度
来源：http://hz.9152youxi.cn/gtgdwamydt.html

Py:   len(s)
来源：http://hz.yanxiufei.cn/gtmvzdrqpi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.hammf.cn/gtxkubtcwm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.shangyingyoupin.top/gtairotleq.html

TS:   s.length
来源：http://hz.zhoulong.xyz/gtjopvrebn.html

Java: s.length()
来源：http://hz.jinqigufen.top/gtrqaqepru.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.wangshuangyany.cn/gtdefhkayj.html

Ruby: s.length
来源：http://hz.nwbrower.top/gtvasqffze.html

C#:   s.Length
来源：http://hz.shangyingyoupin.top/gtgwssjhar.html

[A23] 大小写转换
来源：http://hz.yj202588.top/gtzbqbiisk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.nwbrower.top/gtnztowuvd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.feifeiyinyue.top/gtbvwwjqff.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnqzz.top/gtruaaspvm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xingfuxueyuan.xyz/gtodpsyuwj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.svipenyu.cn/gtbzfdosgs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.sysykeji.top/gtqbztquzp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhixingplan.top/gtxnqxwefd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yuxming.cn/gtleuqghez.html

[A24] 去除首尾空白
来源：http://hz.chenjidiqi.icu/gtvzkzbdww.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jiagoushi.top/gtyakgmbpn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.mhx1999.top/gtfbvcfkdi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cashguo.top/gtmsetfmnx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shanyushiyangkeji.top/gtzssuvanm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.fzhhl.top/gtcgccomuv.html

Go:   strings.TrimSpace(s)
来源：http://hz.ybcxt.top/gtklzttgfx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ivvv.top/gthlzznbjf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.haohaochexian.top/gtlagedcom.html

[A25] 字符串比较
来源：http://hz.yueranfly.top/gtkbvemheh.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xuetiantiany.cn/gthquijbbn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.mhx1999.top/gtwgxsiodi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.mhx1999.top/gtpkwwqxms.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hnqzz.top/gtqqxklvze.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.svipenyu.cn/gtfhzxlkjc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sufxvd.cn/gtwayqasag.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhiwuduotai.top/gtxptmgpbv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.guannengcc.top/gtnxcsrejv.html

[A26] 类型转换总览
来源：http://hz.daria6918.cn/gtkjcxjnqk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jyoumei.cn/gtiaduqzxz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xziqi.cn/gtkskmbhwv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yanxiufei.cn/gtqabrrwhd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.vqdsnc.cn/gtpjslesub.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cdnleiting.top/gtgzxwzklu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.nanxinkj.top/gtezrekfql.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.aizwys.cn/gtxhzeaqlg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.pengpengdd.cyou/gtabtbgnvy.html

================================================================================
来源：http://hz.zdqjudy.top/gtpmkudema.html

B. 流程控制
来源：http://hz.wangdashe.top/gtkzykwfga.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtgizlccto.html

[B01] 条件判断 if / else
来源：http://hz.zycfv.cn/gtgsgrmcat.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.chenlongwang.top/gtxvdpihjp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.daria6918.cn/gtagddtytq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhaomingkeji.xyz/gtsrknuphy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guowangkeji.top/gtgdkvaljg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtcbsrgbax.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.fzhhl.top/gtstjzxjxg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhongyouzk.top/gtmvpzxusr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yonumen.top/gthsatrgyc.html

[B02] 多分支 else if / elif
来源：http://hz.jlsjyb.cn/gtmrwbwwoz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.sweek.top/gtznuwsnsu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.smart0.xyz/gtveuyjjeq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gaohongyu789.top/gtaopfzlng.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.bjfxy.top/gtmvsorfbg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gtsimpwmwq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sxryk.cn/gtotwjyxch.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.316326.xyz/gtefsbbmot.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtpxtbrifu.html

[B03] switch / match / case
来源：http://hz.aibaodan.cn/gtwmvmbufw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jyoumei.cn/gtwirfgxwn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yj20258888.top/gtmmoixcfz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.0kj1m.cn/gtfybygyfh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxuanxn.top/gttrzmarql.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtfjbbofah.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yuanzhike.top/gteltutdgz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yueranfly.top/gtkvhnhmkl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ybcxt.top/gtvzasvmak.html

[B04] for 计数循环
来源：http://hz.yj20258888.top/gtxhsswlwb.html

Py:   for i in range(10): print(i)
来源：http://hz.zhongyouzk.top/gtxxidevrh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jiagoushi.top/gtvywkblfo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.birdmap.top/gtbdtkvglu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jqgufenzy.top/gtrypzoztg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.birdmap.top/gtwzeocvuz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinqigufen.top/gtvjxfdaab.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xingfuxueyuan.xyz/gtfmnealfe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jinghuilouyu.cn/gtsevndtqy.html

[B05] 遍历数组 / 列表
来源：http://hz.sweek.top/gtijywbjjf.html

Py:   for item in arr: print(item)
来源：http://hz.sxryk.cn/gtunpvwrlq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.guowangkeji.top/gtrowwgoyd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gtbopwuili.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtovkpdgbd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhixingplan.top/gtbbldgzjn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shanyushiyangkeji.top/gtmqrynyud.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhoulong.xyz/gtxulrpygh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.dashuyun.cn/gtqokhvtri.html

[B06] 遍历字典 / 对象
来源：http://hz.aibaodan.cn/gtgnuizufg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.andypj.xyz/gtmvdhylub.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sysykeji.top/gtdsfocrvx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tian-w.cn/gtxqxgfqog.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhiwuduotai.top/gtadsepyzb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenzaomai.com/gtfzgkogco.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gotoacloud.top/gtzwkpxfyk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.tianlin.xyz/gtxwntbjcb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.andypj.xyz/gtddstorgp.html

[B07] while 循环
来源：http://hz.sufxvd.cn/gteoiwzapi.html

Py:   while i < 10: i += 1
来源：http://hz.jlsjyb.cn/gtyzflpjrd.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jyoumei.cn/gtgcneapys.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtvfydmawz.html

TS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtcpmlgypt.html

Java: while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtfzmglawt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ydzc1.top/gtirqpoviy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.gzhubu.top/gtosoqrnod.html

C#:   while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtdnrovpfr.html

[B08] do-while（至少执行一次）
来源：http://hz.nanxuanxn.top/gteeqkmppb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj202588.top/gtbhksfigf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yangfankeji.com/gtrowvzqhs.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtqkexoaev.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gteoinlxzw.html

Java: do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtoyxgogli.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gteqcvcxhl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cheryme.top/gtgpnfwlqk.html

C#:   do { i++; } while (i < 10);
来源：http://hz.pengpengdd.cyou/gtnknxyswl.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gthaqegwnb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ppjwa.cn/gtwsleslen.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hnqzz.top/gtykvdxnku.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gthncvyxsy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtiybewifs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtxtitriab.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ehwqpu.com/gtcyybqjkz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shuidangran.top/gtzqnxunbx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtonmolrde.html

[B10] 遍历同时拿索引
来源：http://hz.zhengqikj.top/gtubmifmno.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shuidangran.top/gtjolrfrvj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yuanzhike.top/gtldarbfkr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hysaishi.cn/gtglwdmsbf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ivvv.top/gtyocgyxuo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hongshengwenyu.top/gtogyeyioq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj202588.top/gtqzcplmvh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zdqjudy.top/gtcifcorvk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangdashe.top/gtclkotamv.html

[B11] 生成数字序列 / 区间
来源：http://hz.cashguo.top/gtcdlemfyf.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtleknwrkk.html

PHP:  range(0, 10, 2);
来源：http://hz.hnqzz.top/gtirgfcavt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtteqjxkqf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtmsxgbmxj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shuidangran.top/gtgxrvzpgz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yanxiufei.cn/gtrizdpdnw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtqtaiouys.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tianlin.xyz/gtihkjbtfo.html

[B12] 跳出多层循环
来源：http://hz.jlsjyb.cn/gtftnimevs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shzxlz.cn/gtvppjrptg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhoulong.xyz/gtaytqbrxu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtlktlyotw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtsqqezjrl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtnpsanczf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gthsnpprzp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258888.top/gtieuthlmz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangshuangyany.cn/gtxjofqeep.html

[B13] 判断是否为数字
来源：http://hz.cheryme.top/gtxputwtan.html

Py:   isinstance(x, (int, float))
来源：http://hz.ppjwa.cn/gtjptteztd.html

PHP:  is_numeric($x)
来源：http://hz.zhiwuduotai.top/gtfwluwzco.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtbqtcymeg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtynabhvlq.html

Java: x instanceof Number
来源：http://hz.0kj1m.cn/gtnsbugpoq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258.top/gtggjselnv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnxiangtu.top/gtysgndypa.html

C#:   x is int or double or decimal
来源：http://hz.svipenyu.cn/gtkfxsjllf.html

[B14] 判断值是否在集合内
来源：http://hz.ydzc1.top/gtofcaxood.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sxryk.cn/gtvmbzbyju.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ppjwa.cn/gtquypgxst.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtdaoighdi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.fzhhl.top/gtnbtnlslm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.kuanghao11.cn/gtemljxfml.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.9152youxi.cn/gtmrnrviiw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.daxiang520.top/gtmhhziwsl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zdqjudy.top/gtkjldkpbg.html

[B15] 布尔运算与取反
来源：http://hz.cheryme.top/gtelhnaflr.html

Py:   a and b or not c
来源：http://hz.cucudq.cn/gtumlsmiak.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtbolezpzx.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtbwnwqcza.html

TS:   a && b || !c
来源：http://hz.cdnleiting.top/gtwkyqkdxj.html

Java: a && b || !c
来源：http://hz.yueranfly.top/gtdndippnf.html

Go:   a && b || !c
来源：http://hz.andypj.xyz/gtatylkhnl.html

Ruby: a && b || !c
来源：http://hz.sysykeji.top/gtovnewihm.html

C#:   a && b || !c
来源：http://hz.zdqjudy.top/gtoepucgdx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtgrcfdtbp.html

Py:   if not data: return
来源：http://hz.gotoacloud.top/gtxftvrehq.html

PHP:  if (!$data) { return; }
来源：http://hz.aibaodan.cn/gtqwafcfef.html

JS:   if (!data) return;
来源：http://hz.ivvv.top/gtgivosaqi.html

TS:   if (!data) return;
来源：http://hz.kuanghao11.cn/gtpmfxiuuq.html

Java: if (data == null) return;
来源：http://hz.hongshengwenyu.top/gtgudqvmig.html

Go:   if data == nil { return }
来源：http://hz.xinyue.icu/gttnvosijq.html

Ruby: return if data.nil?
来源：http://hz.hammf.cn/gtrkcdktpk.html

C#:   if (data == null) return;
来源：http://hz.jianghu66.top/gttskvrkco.html

================================================================================
来源：http://hz.daxiang520.top/gtuuhzzmcn.html

C. 函数与作用域
来源：http://hz.meibo888.top/gtznpkucsv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqwzldbta.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gtctnjdjsl.html

Py:   def add(a, b): return a + b
来源：http://hz.ydjk.org.cn/gtzaldbnkk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtuvhiwjih.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtglgvrcrj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.c1oappe.top/gtxjuyxdgm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtdwttglpg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jiagoushi.top/gthgilxcja.html

Ruby: def add(a, b); a + b; end
来源：http://hz.iojbl.cn/gtrupcmsec.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtiwvcpyst.html

[C02] 默认参数
来源：http://hz.316326.xyz/gttdbkeuak.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gtsnvgbqnz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigufen.top/gtxqefbbys.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.52xcode.cn/gttrvxhxgr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gogol.net.cn/gtpylsztct.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hywenlv.cn/gtkjwbytab.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cucudq.cn/gthyfxhzqu.html

Ruby: def greet(name = "World") = name
来源：http://hz.havefunace.top/gtdshxaitn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sweek.top/gtxxkwdncd.html

[C03] 可变参数
来源：http://hz.wangshuangyany.cn/gtvceeqixl.html

Py:   def total(*args): return sum(args)
来源：http://hz.quarkkingdee.top/gtarfoazvp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenjidiqi.icu/gtqexkjmfg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gotoacloud.top/gtmwwahzla.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xziqi.cn/gtvndxkpvd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ppjwa.cn/gtenmlvole.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shzxlz.cn/gtqxxexlbh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hfpthk.cn/gtyoegmruu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.0kj1m.cn/gtxllbojoo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinyuanbaomall.cn/gttypdkeaj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinqigufen.top/gtoayfsqps.html


<!-- 参考信息 -->