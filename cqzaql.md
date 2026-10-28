代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.iojbl.cn/gtmopgfxxd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.iojbl.cn/gtdjhgrnjb.html

TS:   if (!x) {}
来源：http://hz.yj20258888.top/gtgmcuilpx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.cheryme.top/gtzghqaytn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.cheryme.top/gtdyejhgcr.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.316326.xyz/gtnxueqjbm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ivvv.top/gtibjevfmp.html

[A17] 位运算
来源：http://hz.birdmap.top/gtqcwkdkdw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtctsbygmk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.gzhubu.top/gtbythfgjy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gtklknvrdl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtbkjhytzn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258888.top/gtvmsejypj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtuplfnqmt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenzaomai.com/gtlrwqsdjj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtlryqgvkh.html

[A18] 字符与 ASCII 码互转
来源：http://hz.fengsongda.top/gtstyomaba.html

Py:   ord("A"); chr(65)
来源：http://hz.cashguo.top/gtumpqttsk.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhoulong.xyz/gtqtzdlrli.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cdnleiting.top/gtxobuhkzr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jianghu66.top/gtmpmnpouv.html

Java: (int) 'A'; (char) 65
来源：http://hz.hfpthk.cn/gtlzqdiquw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.aibaodan.cn/gtwcitdbyo.html

Ruby: "A".ord; 65.chr
来源：http://hz.jinyuanbaomall.cn/gtepuyzgmu.html

C#:   (int)'A'; (char)65
来源：http://hz.9152youxi.cn/gttzkxrdib.html

[A19] 交换两个变量
来源：http://hz.yvedp.cn/gtbhzercnp.html

Py:   a, b = b, a
来源：http://hz.0kj1m.cn/gtlqfhxjso.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yvedp.cn/gtkzpvztou.html

JS:   [a, b] = [b, a];
来源：http://hz.hywenlv.cn/gtoythfvez.html

TS:   [a, b] = [b, a];
来源：http://hz.cqqwz.cn/gtkvbehciw.html

Java: int t = a; a = b; b = t;
来源：http://hz.smart0.xyz/gtnybbpshe.html

Go:   a, b = b, a
来源：http://hz.yonumen.top/gtqbakmoaa.html

Ruby: a, b = b, a
来源：http://hz.jiagoushi.top/gtcdusjztx.html

C#:   (a, b) = (b, a);
来源：http://hz.tian-w.cn/gtczowleao.html

[A20] 读取标准输入
来源：http://hz.gzhubu.top/gtwhmbmxyx.html

Py:   name = input("请输入：")
来源：http://hz.vqdsnc.cn/gtepcliwlf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.pengpengdd.cyou/gtpuvijner.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yj202588.top/gtvwtjyrke.html

TS:   // Node.js：readline 模块
来源：http://hz.c1oappe.top/gtuswmrrqm.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.quarkkingdee.top/gtxuobxmmc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.kuanghao11.cn/gttodurlvi.html

Ruby: gets.chomp
来源：http://hz.zhijiandao.cn/gtnsoxaxsf.html

C#:   Console.ReadLine();
来源：http://hz.smart0.xyz/gtfzglubto.html

[A21] 保留指定小数位输出
来源：http://hz.dashuyun.cn/gtycphnezc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jiagoushi.top/gtkvtgmbyn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gtduuyvyck.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hfpthk.cn/gtfuzthaph.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yuanzhike.top/gtlazrnfis.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtnsronusg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.nwbrower.top/gtykqxpgop.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.guowangkeji.top/gtkmuoywpf.html

C#:   3.14159.ToString("F2")
来源：http://hz.svipenyu.cn/gtltmbraox.html

[A22] 获取字符串长度
来源：http://hz.birdmap.top/gtoeceaesf.html

Py:   len(s)
来源：http://hz.yonumen.top/gtsukhloxj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ywan-chungtsiang.top/gtbfvjepoq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.quarkkingdee.top/gtmwakxjzt.html

TS:   s.length
来源：http://hz.gogol.net.cn/gtwdgjtgri.html

Java: s.length()
来源：http://hz.zhaomingkeji.xyz/gtmbjaoibt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.ppjwa.cn/gtgxoannbt.html

Ruby: s.length
来源：http://hz.chenlongwang.top/gtpiteooht.html

C#:   s.Length
来源：http://hz.wangshuangyany.cn/gtppoqcyls.html

[A23] 大小写转换
来源：http://hz.zhongyouzk.top/gtuawakttt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hfpthk.cn/gtoigeslsv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.shzxlz.cn/gtfygtlcgr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.vqdsnc.cn/gtwscyzbhp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sufxvd.cn/gtkxqrpkdi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.xingfuxueyuan.xyz/gtbpbniybh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hammf.cn/gtxvkygbqo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenzaomai.com/gtqnkiflvo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zycfv.cn/gtxucepdcl.html

[A24] 去除首尾空白
来源：http://hz.pycfn.com/gtbwwkreir.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daria6918.cn/gttyqvaeec.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hongshengwenyu.top/gtypeqyspj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hysaishi.cn/gtlepqqasu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tianlin.xyz/gtnsdbimrt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xingfuxueyuan.xyz/gtkjbppgpq.html

Go:   strings.TrimSpace(s)
来源：http://hz.chenzaomai.com/gtsjxhfgyi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yuxming.cn/gtjdutarhc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.tian-w.cn/gtemivvaxo.html

[A25] 字符串比较
来源：http://hz.52xcode.cn/gtzpqqmuqd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.0kj1m.cn/gtafzhvnka.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shuidangran.top/gtedwzqfnp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gttwjtfhwz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj20258888.top/gtbdorukvf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zhaomingkeji.xyz/gtgzfkrywy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hfpthk.cn/gtpzpamjpz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xuanzx.com/gtahtkisjt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cheryme.top/gtqptnjatz.html

[A26] 类型转换总览
来源：http://hz.zhaomingkeji.xyz/gtljoceszt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jyoumei.cn/gtlqcnuexy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.pycfn.com/gthwsbcyfc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.wangdashe.top/gtvfbrlatt.html

TS:   Number() String() Boolean() x as number
来源：http://hz.smart0.xyz/gtuptgggrv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.meibo888.top/gtzwpzncgp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yuanzhike.top/gtitngabud.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yuxming.cn/gthmpuerba.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.bjfxy.top/gtqlftshhk.html

================================================================================
来源：http://hz.hfpthk.cn/gtjsamminn.html

B. 流程控制
来源：http://hz.xuanzx.com/gtmqynsrzh.html

================================================================================
来源：http://hz.yanxiufei.cn/gtaspfrgep.html

[B01] 条件判断 if / else
来源：http://hz.svipenyu.cn/gtdjmgzlcu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.sysykeji.top/gttetrghjz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shuidangran.top/gtrjdbarhw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtilxjzehp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtobtmniev.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.aizwys.cn/gthekaruwt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhixingplan.top/gtesrpmlqh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.bjfxy.top/gtnjmccueg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258.top/gtqrykhayj.html

[B02] 多分支 else if / elif
来源：http://hz.sufxvd.cn/gtvszfrzqq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.tian-w.cn/gtlzqezadr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.316326.xyz/gtejubefkg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gtbdkgjbjr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuxming.cn/gtzaqategs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tanke756.top/gtkknlkjkb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.tianlin.xyz/gtjfabgzsg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.tian-w.cn/gtenftztag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gtovyfgbgp.html

[B03] switch / match / case
来源：http://hz.wangshuangyany.cn/gtnzrfahrk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.tianlin.xyz/gtzbohvmty.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gtatkbevwa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtotpybnzi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.mhx1999.top/gthprtrobz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtresavfms.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.daria6918.cn/gtjufiffyl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.meibo888.top/gtjcdelall.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cdnleiting.top/gtjzyguozr.html

[B04] for 计数循环
来源：http://hz.jinqigufen.top/gthpgsmbgn.html

Py:   for i in range(10): print(i)
来源：http://hz.zycfv.cn/gtgckvwnjm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xuanzx.com/gttqydwirr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtzrnpamni.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhiwuduotai.top/gtbowcksus.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.birdmap.top/gtstihtwxg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cheryme.top/gtlmvnfhei.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daria6918.cn/gttzhtdfor.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zycfv.cn/gtqedvswqx.html

[B05] 遍历数组 / 列表
来源：http://hz.guowangkeji.top/gtvevbycdv.html

Py:   for item in arr: print(item)
来源：http://hz.zhiwuduotai.top/gtvzyhijod.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenlongwang.top/gtdyjwriez.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.dianchejie.cn/gtfwcmaoiy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.svipenyu.cn/gtknedoktg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.nanxuanxn.top/gtzaxmaabo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.feifeiyinyue.top/gtoyqlxuii.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cheryme.top/gtnjdoifhr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangdashe.top/gtuyvnclhf.html

[B06] 遍历字典 / 对象
来源：http://hz.yj202588.top/gtxekyurlr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sysykeji.top/gtkwnpduyx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.vqdsnc.cn/gtbqlpsogx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cashguo.top/gtwmzredqd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj202588.top/gtrnabpqoz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj20258.top/gtzapqtagk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.tanke756.top/gttzxcizji.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jqgufenzy.top/gtqslrcqon.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xinyue.icu/gtxpuaywdi.html

[B07] while 循环
来源：http://hz.wangdashe.top/gtoenhgyqn.html

Py:   while i < 10: i += 1
来源：http://hz.zhengqikj.top/gtuwivawev.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xingfuxueyuan.xyz/gtvcygfpja.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtlmybpski.html

TS:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtrilyayvg.html

Java: while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtrnviksmm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xingfuxueyuan.xyz/gtdutmxntq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ehwqpu.com/gtorgytjqv.html

C#:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtjsemezub.html

[B08] do-while（至少执行一次）
来源：http://hz.zycfv.cn/gtobjlabcw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.tian-w.cn/gtaohkiqgh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.tian-w.cn/gtoxoudttj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtowknarvv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtxbuzsgjr.html

Java: do { i++; } while (i < 10);
来源：http://hz.hongshengwenyu.top/gtrpxwpzoc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gogol.net.cn/gtzkuiutis.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shangyingyoupin.top/gtkttufuxy.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhengqikj.top/gtyzxvwkwj.html

[B09] break 与 continue
来源：http://hz.gaohongyu789.top/gtzjsivyqs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yanxiufei.cn/gtkqdboxlr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258.top/gtykakzskg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtympmarvo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtptrdbjou.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtamfenoop.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ehwqpu.com/gtgzexitgx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.birdmap.top/gtbfwnmwpc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtffiikcey.html

[B10] 遍历同时拿索引
来源：http://hz.ydzc1.top/gtjqomsnrk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.pycfn.com/gtvabkgbrl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shuidangran.top/gttyaiaedx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgfzy.top/gtsuscfjas.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.52xcode.cn/gtzyayilwi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jyoumei.cn/gtuuobejml.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.kuanghao11.cn/gtalhyjlcw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenzaomai.com/gtbdkwoqrm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dianchejie.cn/gttvdeqdok.html

[B11] 生成数字序列 / 区间
来源：http://hz.hammf.cn/gtfswfjhjd.html

Py:   list(range(0, 10, 2))
来源：http://hz.yangfankeji.com/gtodofktba.html

PHP:  range(0, 10, 2);
来源：http://hz.xylfe.cn/gthaqmtlky.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.snrcjt.cn/gtpmsprmzd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gthkwtpvvt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.quarkkingdee.top/gtrixnlcta.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gtltojllif.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shuidangran.top/gtzkozhrkl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigfzy.top/gtlcmdvapq.html

[B12] 跳出多层循环
来源：http://hz.yuanzhike.top/gtxmlbixhc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhengqikj.top/gtmaebifln.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yj20258.top/gtthjgvsjj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gtdxoxgpcg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj202588.top/gtyxiefeab.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtujiiwoeb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.redwolf501.top/gtusqimcfo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.birdmap.top/gtasabkpza.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gzhubu.top/gtsbhfpcdm.html

[B13] 判断是否为数字
来源：http://hz.zhengqikj.top/gtudmuuukl.html

Py:   isinstance(x, (int, float))
来源：http://hz.havefunace.top/gtvcmlhkbg.html

PHP:  is_numeric($x)
来源：http://hz.shuidangran.top/gtodhwbfkw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtihwsatib.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtcdfgwfrb.html

Java: x instanceof Number
来源：http://hz.xuanzx.com/gtahhmzlhm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jyoumei.cn/gtnwaxlrgs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.fengsongda.top/gtxmshpwrr.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtwxtekrcu.html

[B14] 判断值是否在集合内
来源：http://hz.316326.xyz/gtejpkjayn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.haohaochexian.top/gtqrzzumgu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtjxsicgeb.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtopjfvbag.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenlongwang.top/gtrlfsvkpk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guowangkeji.top/gtzvsjxlrk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.316326.xyz/gthurxkzhw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.smart0.xyz/gtelyqmlea.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hongshengwenyu.top/gttgglyskf.html

[B15] 布尔运算与取反
来源：http://hz.yvedp.cn/gtoazaywzx.html

Py:   a and b or not c
来源：http://hz.hammf.cn/gtkpjmwfap.html

PHP:  $a && $b || !$c
来源：http://hz.zhoulong.xyz/gtqhsnchkh.html

JS:   a && b || !c
来源：http://hz.bjfxy.top/gtwareyweu.html

TS:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtymlgyull.html

Java: a && b || !c
来源：http://hz.yuanzhike.top/gtuesbivxu.html

Go:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtdoipegjx.html

Ruby: a && b || !c
来源：http://hz.aibaodan.cn/gtybcfqjyy.html

C#:   a && b || !c
来源：http://hz.yj20258888.top/gticyaleck.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.aizwys.cn/gtzfyprypw.html

Py:   if not data: return
来源：http://hz.hongshengwenyu.top/gtorwzouly.html

PHP:  if (!$data) { return; }
来源：http://hz.dashuyun.cn/gtvzrqzevu.html

JS:   if (!data) return;
来源：http://hz.sweek.top/gtitaxefat.html

TS:   if (!data) return;
来源：http://hz.jianghu66.top/gtglfqxzmq.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gtyakcztfh.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtzvessamz.html

Ruby: return if data.nil?
来源：http://hz.xylfe.cn/gtcbjaizfc.html

C#:   if (data == null) return;
来源：http://hz.hywenlv.cn/gtccfjvgaw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gttupkikao.html

C. 函数与作用域
来源：http://hz.jiagoushi.top/gtjcssvxyg.html

================================================================================
来源：http://hz.gotoacloud.top/gtoszytloy.html

[C01] 定义函数
来源：http://hz.bjfxy.top/gtoffgyfdy.html

Py:   def add(a, b): return a + b
来源：http://hz.yj20258.top/gtzievcywv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtpjlfzjnz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtouzcsqwb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtpskcdwfb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtjpwlmkyq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigufen.top/gtvkmiypte.html

Ruby: def add(a, b); a + b; end
来源：http://hz.fengsongda.top/gtdfkgdxxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gtmmmhvaka.html

[C02] 默认参数
来源：http://hz.ppjwa.cn/gtcyyxouws.html

Py:   def greet(name="World"): return name
来源：http://hz.hongshengwenyu.top/gtlgzwqnvk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.9152youxi.cn/gthsmuaekj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj202588.top/gtxqyngszt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtdxfvwdai.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxinkj.top/gtpcuwtaog.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgfzy.top/gtahtbxbti.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gtdfkoinct.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.52xcode.cn/gtdbvqjgkb.html

[C03] 可变参数
来源：http://hz.jyoumei.cn/gttxycmljo.html

Py:   def total(*args): return sum(args)
来源：http://hz.fzhhl.top/gtelfykkon.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.svipenyu.cn/gtczftwdrl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtiqsmrwct.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtcuatyqyk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gzhubu.top/gtdulglyqq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tanke756.top/gtunhmpmks.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dianchejie.cn/gtqszncjip.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gtsebsugeb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sysykeji.top/gtgdqgeqif.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinghuilouyu.cn/gtolvervcf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenjidiqi.icu/gtmfihfmxy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtfobhzwqi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jqgufenzy.top/gtbkwnwsbe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinghuilouyu.cn/gtfzlvmqjf.html

Go:   // 无：用配置结构体参数
来源：http://hz.tanke756.top/gthdtbzmja.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtmuccsjad.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtmuayvrqo.html

[C05] 返回多个值
来源：http://hz.ydjk.org.cn/gthbewxzec.html

Py:   return a, b
来源：http://hz.dianchejie.cn/gtkdghuluo.html

PHP:  return [$a, $b];
来源：http://hz.ywan-chungtsiang.top/gtsjwjmpxb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shzxlz.cn/gttgbrrmdq.html

TS:   return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtvlrowyih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zdqjudy.top/gtyeadixam.html

Go:   return a, b
来源：http://hz.xziqi.cn/gtyrwtchtp.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtewwnpkso.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtjpgxqssd.html

[C06] 匿名函数 / lambda
来源：http://hz.cashguo.top/gtmzyiwgyi.html

Py:   square = lambda x: x * x
来源：http://hz.gogol.net.cn/gtarhjgwfg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yvedp.cn/gtbfkbqkkm.html

JS:   const square = x => x * x;
来源：http://hz.feifeiyinyue.top/gthuvihyxy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sufxvd.cn/gtlyxzatij.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.iojbl.cn/gtwnqgzgxe.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangtech.top/gtbxpzkcie.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jianghu66.top/gttousjpxc.html


<!-- 参考信息 -->