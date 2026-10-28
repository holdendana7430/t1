代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.dianchejie.cn/gtaejzlbqp.html

TS:   const value = data ?? "默认值";
来源：http://hz.yj202588.top/gtcwmqsdbw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.birdmap.top/gtpkxkaezt.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.9152youxi.cn/gtykmhklir.html

Ruby: value = data || "默认值"
来源：http://hz.sxryk.cn/gtdepmdyds.html

C#:   var value = data ?? "默认值";
来源：http://hz.guannengcc.top/gtchnhlbga.html

[A16] 真假值判断规则
来源：http://hz.aizwys.cn/gtewhbdleg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.gaohongyu789.top/gtqugpupka.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.wangshuangyany.cn/gtzlpwemjv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xuanzx.com/gtqsnkjgvw.html

TS:   if (!x) {}
来源：http://hz.nwbrower.top/gtdihqagjm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.chenlongwang.top/gtfjtkquko.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.nwbrower.top/gtvnzekgwk.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.chenjidiqi.icu/gtiqorfhqw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.svipenyu.cn/gtphmhumez.html

[A17] 位运算
来源：http://hz.jiagoushi.top/gttxiexsin.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtrkfmzeuh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.havefunace.top/gtblnoqowk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gtowkzkcwo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yongpay.top/gtyvsgqksa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gogol.net.cn/gtzhohqtjo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtgsogvqut.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtncjjqnew.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gttqsnbspy.html

[A18] 字符与 ASCII 码互转
来源：http://hz.sxryk.cn/gtihbmjpzj.html

Py:   ord("A"); chr(65)
来源：http://hz.kuanghao11.cn/gtjmvfesao.html

PHP:  ord("A"); chr(65)
来源：http://hz.gzhubu.top/gtzfngqwsj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sysykeji.top/gtzlkvptjz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gotoacloud.top/gtknzgzvwp.html

Java: (int) 'A'; (char) 65
来源：http://hz.gaohongyu789.top/gtqefxbloi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jyoumei.cn/gtwpahzvpx.html

Ruby: "A".ord; 65.chr
来源：http://hz.pycfn.com/gtkdnjmzim.html

C#:   (int)'A'; (char)65
来源：http://hz.meibo888.top/gtdtvnxkqw.html

[A19] 交换两个变量
来源：http://hz.guannengcc.top/gtcrbmcyrf.html

Py:   a, b = b, a
来源：http://hz.mhx1999.top/gtqkkdbdvp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yuanzhike.top/gtndubxbbo.html

JS:   [a, b] = [b, a];
来源：http://hz.hnxiangtu.top/gtofinvpst.html

TS:   [a, b] = [b, a];
来源：http://hz.shuidangran.top/gtaorqtete.html

Java: int t = a; a = b; b = t;
来源：http://hz.hammf.cn/gtlojkaqwp.html

Go:   a, b = b, a
来源：http://hz.tanke756.top/gtormfcmmk.html

Ruby: a, b = b, a
来源：http://hz.yuanzhike.top/gtsymnfjya.html

C#:   (a, b) = (b, a);
来源：http://hz.yvedp.cn/gttstmnbao.html

[A20] 读取标准输入
来源：http://hz.wangshuangyany.cn/gtbidypyfr.html

Py:   name = input("请输入：")
来源：http://hz.snrcjt.cn/gttoxbshqf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hywenlv.cn/gteyxnttgo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.guannengcc.top/gtktqodrsi.html

TS:   // Node.js：readline 模块
来源：http://hz.jlsjyb.cn/gtbzdxcouc.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hnxiangtu.top/gtbbkfyadq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.quarkkingdee.top/gttykorwff.html

Ruby: gets.chomp
来源：http://hz.zhijiandao.cn/gtjfruadef.html

C#:   Console.ReadLine();
来源：http://hz.chenjidiqi.icu/gtsvnheiqx.html

[A21] 保留指定小数位输出
来源：http://hz.jinyuanbaomall.cn/gtsijytfhw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zdqjudy.top/gtpeybihms.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jinghuilouyu.cn/gtvsjdhtfr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ybcxt.top/gthywimrcl.html

TS:   (3.14159).toFixed(2)
来源：http://hz.cheryme.top/gtxqteemta.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.xylfe.cn/gtespnnngf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shanyushiyangkeji.top/gtgypdcffe.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangshuangyany.cn/gtkhbnfiwn.html

C#:   3.14159.ToString("F2")
来源：http://hz.zycfv.cn/gtodiwuxor.html

[A22] 获取字符串长度
来源：http://hz.zhiwuduotai.top/gtswyuajcd.html

Py:   len(s)
来源：http://hz.jinqigufen.top/gtgdlabuyr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.cucudq.cn/gtuegmbabc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.nwbrower.top/gtrerpemkq.html

TS:   s.length
来源：http://hz.hnxiangtu.top/gtyheiuxvu.html

Java: s.length()
来源：http://hz.havefunace.top/gtydnckryh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.nwbrower.top/gtkgbkppft.html

Ruby: s.length
来源：http://hz.hysaishi.cn/gtmowjarqf.html

C#:   s.Length
来源：http://hz.hnqzz.top/gttxzshsnm.html

[A23] 大小写转换
来源：http://hz.cqqwz.cn/gtrhhvgscr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yj202588.top/gtvailaxhx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.sufxvd.cn/gtigfkbvrp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hywenlv.cn/gtsokmwvwp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zycfv.cn/gtcdqnyfwz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.52xcode.cn/gtgxeiwmwo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhiwuduotai.top/gtooohdeji.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhixingplan.top/gtuscbscog.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gotoacloud.top/gtptfhpnux.html

[A24] 去除首尾空白
来源：http://hz.fengsongda.top/gtwcjlkbmx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.nanxuanxn.top/gthlkxqyfc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.andypj.xyz/gttvfvxjhz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.andypj.xyz/gtaudcugsh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shanyushiyangtech.top/gtpybxjsvc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shzxlz.cn/gtqjobnabc.html

Go:   strings.TrimSpace(s)
来源：http://hz.hongshengwenyu.top/gtdaaonvwc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cashguo.top/gttzfsxwpj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.0kj1m.cn/gtbhlfacyg.html

[A25] 字符串比较
来源：http://hz.svipenyu.cn/gtonpncwwo.html

Py:   s1 == s2; s1 != s2
来源：http://hz.sysykeji.top/gtszkitedj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jinyuanbaomall.cn/gttgevogll.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.316326.xyz/gtgnxpbbcj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgfzy.top/gtgvvtjnyz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yanxiufei.cn/gtnbvktlmt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yj20258.top/gtybyvyige.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yj202588.top/gthutarxdj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yvedp.cn/gthrmzzxol.html

[A26] 类型转换总览
来源：http://hz.jianghu66.top/gtvrobscir.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhongyouzk.top/gtdngfjrpu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jinghuilouyu.cn/gtubirdggw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.chenlongwang.top/gtzmlzhjrs.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yanxiufei.cn/gtongqwksm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xuetiantiany.cn/gtfsitqwms.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhiwuduotai.top/gtqjvpyedn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yonumen.top/gtdvyynpcl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shuidangran.top/gtzaceybhi.html

================================================================================
来源：http://hz.yj202588.top/gtpbbouosp.html

B. 流程控制
来源：http://hz.zhijiandao.cn/gtbpsddmso.html

================================================================================
来源：http://hz.nwbrower.top/gtvmcdbrnp.html

[B01] 条件判断 if / else
来源：http://hz.tianlin.xyz/gtqhwweqte.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.birdmap.top/gtynimndbw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shanyushiyangtech.top/gtdufmfdcz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtoktwvkbn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtpjdqirhp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtqyshzwty.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cheryme.top/gtxynwdrfn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yueranfly.top/gttghzhifo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtsvnuojro.html

[B02] 多分支 else if / elif
来源：http://hz.sxryk.cn/gtedecgjzq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yuanzhike.top/gtafwkmwjw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.cdnleiting.top/gtzrbdplyl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtjypwztfh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gtqqffcbzx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gaohongyu789.top/gtdnphpplz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shzxlz.cn/gtxiytcxpc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.wangdashe.top/gtgigdcdbz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtanbpfrej.html

[B03] switch / match / case
来源：http://hz.sufxvd.cn/gtnfdhvyrj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xinyue.icu/gthiljfhkb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yongpay.top/gtztyhplpd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sweek.top/gternjhugy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.vqdsnc.cn/gtjdsaqbma.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.haohaochexian.top/gtjllrdxfd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.aibaodan.cn/gtewicagey.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ywan-chungtsiang.top/gtujcxgjpm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yj20258.top/gtzkapfuik.html

[B04] for 计数循环
来源：http://hz.yj20258.top/gtcqvtddih.html

Py:   for i in range(10): print(i)
来源：http://hz.jinqigufen.top/gtduxpwjim.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jinqigufen.top/gtvamhwydr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangdashe.top/gtzgdjbfbo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhiwuduotai.top/gtcblkemue.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shzxlz.cn/gtjxepfrpj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.nanxuanxn.top/gtswjycxnz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xinyue.icu/gtfacepdhl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hywenlv.cn/gtevagppmn.html

[B05] 遍历数组 / 列表
来源：http://hz.feifeiyinyue.top/gtnwzvrpwi.html

Py:   for item in arr: print(item)
来源：http://hz.nanxinkj.top/gtjftxvbnc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gzhubu.top/gtssjtjslf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shuidangran.top/gtxnnxlgqy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtoxrxfovn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.chenjidiqi.icu/gtcpkpaata.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yonumen.top/gtujcrgrih.html

Ruby: arr.each { |item| puts item }
来源：http://hz.bjfxy.top/gtkqhnogbw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hammf.cn/gtygwzgjgp.html

[B06] 遍历字典 / 对象
来源：http://hz.pengpengdd.cyou/gtchkbnako.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.9152youxi.cn/gtilmhoosg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yvedp.cn/gtbddkzsml.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.quarkkingdee.top/gtabsguurj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.wangshuangyany.cn/gtdugfhqbd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.dianchejie.cn/gtjdslbfdm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.chenlongwang.top/gtbqbhnblo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.aibaodan.cn/gtithtjbus.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shangyingyoupin.top/gtsmbvgxxm.html

[B07] while 循环
来源：http://hz.daxiang520.top/gtzhvltyat.html

Py:   while i < 10: i += 1
来源：http://hz.gotoacloud.top/gtgftndqju.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.wangshuangyany.cn/gtyudxxebj.html

JS:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtjatqvblm.html

TS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtcrrwgxuo.html

Java: while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtxnehzatr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daria6918.cn/gtiircpagh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.tian-w.cn/gtnkeswzbn.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtrfzdhbsl.html

[B08] do-while（至少执行一次）
来源：http://hz.pycfn.com/gtimumnsih.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.haohaochexian.top/gtnywgtesc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtzwqmmrso.html

JS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtofrxgwpz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinyuanbaomall.cn/gtlagtvwnu.html

Java: do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtpgiatqie.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gotoacloud.top/gtljvvqxuk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.dashuyun.cn/gtvmlswcsc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtbxnmgrfl.html

[B09] break 与 continue
来源：http://hz.shuidangran.top/gtnbqdnldu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gotoacloud.top/gtxlpuddfz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.0kj1m.cn/gtfztqidkp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtnwdcigff.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtlrswfxsw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtzismblxs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.wangdashe.top/gtuxaardfl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shzxlz.cn/gtbrwrmsgb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtzbdakdmk.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtjqxpnndi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj20258888.top/gtzusxwumh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cqqwz.cn/gtobrumsju.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gthwumjhsz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ywan-chungtsiang.top/gtbqbewwei.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.aizwys.cn/gtoeaduxdi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.smart0.xyz/gtfwxvvpwd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.0kj1m.cn/gtipejlxuk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gotoacloud.top/gtqmvbuivp.html

[B11] 生成数字序列 / 区间
来源：http://hz.zycfv.cn/gtuadtupra.html

Py:   list(range(0, 10, 2))
来源：http://hz.vqdsnc.cn/gtlcdtgjwb.html

PHP:  range(0, 10, 2);
来源：http://hz.cqqwz.cn/gtgnsvqgag.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zdqjudy.top/gtkppemhyu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtvwnnfdml.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.birdmap.top/gtjttlsxcx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daxiang520.top/gtlydshkae.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenzaomai.com/gtcpvwrthp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dashuyun.cn/gthwypjole.html

[B12] 跳出多层循环
来源：http://hz.hnqzz.top/gtpufqvhaf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yj202588.top/gtofzmprax.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tianlin.xyz/gtnczlwmso.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtshtfhuyh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtaiiurpjm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtkdagsijz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhixingplan.top/gttfobhwzu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yongpay.top/gtnoxggqwb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.quarkkingdee.top/gtwhivcuyj.html

[B13] 判断是否为数字
来源：http://hz.birdmap.top/gthzqayqxe.html

Py:   isinstance(x, (int, float))
来源：http://hz.guannengcc.top/gttymcudma.html

PHP:  is_numeric($x)
来源：http://hz.jqgfzy.top/gtdfyqcibi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtznmsmbcw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtrugmuwtw.html

Java: x instanceof Number
来源：http://hz.shzxlz.cn/gtuwedofxa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinghuilouyu.cn/gtwgkshhlq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xinyue.icu/gtbrwzlade.html

C#:   x is int or double or decimal
来源：http://hz.gogol.net.cn/gthfgfqcwd.html

[B14] 判断值是否在集合内
来源：http://hz.ivvv.top/gtoeuofzji.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.0kj1m.cn/gtzhmppuql.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.haohaochexian.top/gtqlelyxba.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tianlin.xyz/gtpkapaaak.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtrpokxvqe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.aibaodan.cn/gtggqipekm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigufen.top/gtjltbrvxg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yanxiufei.cn/gtjmbcajhr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.fzhhl.top/gtvacrusos.html

[B15] 布尔运算与取反
来源：http://hz.9152youxi.cn/gtfwqlviaw.html

Py:   a and b or not c
来源：http://hz.zhiwuduotai.top/gtuclnejau.html

PHP:  $a && $b || !$c
来源：http://hz.zhiwuduotai.top/gtbahwykmx.html

JS:   a && b || !c
来源：http://hz.tian-w.cn/gtxynxujln.html

TS:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtsblvnopj.html

Java: a && b || !c
来源：http://hz.daxiang520.top/gtdnuedaoz.html

Go:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtqucwikxb.html

Ruby: a && b || !c
来源：http://hz.ydjk.org.cn/gtptpvqmfy.html

C#:   a && b || !c
来源：http://hz.zhixingplan.top/gtbrgriaxh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtxhlbopim.html

Py:   if not data: return
来源：http://hz.gaohongyu789.top/gtlplfyvih.html

PHP:  if (!$data) { return; }
来源：http://hz.birdmap.top/gtzidtencc.html

JS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtkhsjmbzt.html

TS:   if (!data) return;
来源：http://hz.xziqi.cn/gtkctposaj.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtdzcplkfh.html

Go:   if data == nil { return }
来源：http://hz.feifeiyinyue.top/gtpegfpcwx.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gtvxblpucz.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gthmvkeqfl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcsgtidcm.html

C. 函数与作用域
来源：http://hz.shzxlz.cn/gtcbqaefjf.html

================================================================================
来源：http://hz.shuidangran.top/gthojlruzj.html

[C01] 定义函数
来源：http://hz.jinghuilouyu.cn/gtlqvupnew.html

Py:   def add(a, b): return a + b
来源：http://hz.316326.xyz/gtphlezese.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtsbygixzt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtcniulzgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtdbkmpuor.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtwdxuytom.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangdashe.top/gtfrcgsszl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtbqcxwftk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtcbqbvvvf.html

[C02] 默认参数
来源：http://hz.dashuyun.cn/gthycdyqud.html

Py:   def greet(name="World"): return name
来源：http://hz.jyoumei.cn/gttbfnpnpr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhiwuduotai.top/gtkaridbkf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtgswiyvnv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aizwys.cn/gtjyafsqyw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnqzz.top/gtrkksmchp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ivvv.top/gtloyuqwtz.html

Ruby: def greet(name = "World") = name
来源：http://hz.ivvv.top/gtqcxdrrtm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cdnleiting.top/gtkupajfqw.html

[C03] 可变参数
来源：http://hz.hywenlv.cn/gtnxxczdpz.html

Py:   def total(*args): return sum(args)
来源：http://hz.haohaochexian.top/gtmwmghzfn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ppjwa.cn/gtenfsqnnw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtrodywmli.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gttanmtwet.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sxryk.cn/gtuswbhsxf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnxiangtu.top/gtfcscujoj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nwbrower.top/gtetewmvfm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xziqi.cn/gtiqfnbade.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sysykeji.top/gtcdhdngam.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cqqwz.cn/gtdbzrbcya.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhaomingkeji.xyz/gtjiwzhpww.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.havefunace.top/gtqnhvjcdf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daria6918.cn/gtxjggsvim.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnqzz.top/gttldgfeqx.html

Go:   // 无：用配置结构体参数
来源：http://hz.xziqi.cn/gtkmgrshlz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtjjxzxjlh.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtapnnprfl.html

[C05] 返回多个值
来源：http://hz.fengsongda.top/gtfsppgprp.html

Py:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtywzdmfsj.html

PHP:  return [$a, $b];
来源：http://hz.redwolf501.top/gtnhgbmoqf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydjk.org.cn/gtangvmrjv.html

TS:   return { a, b };
来源：http://hz.yvedp.cn/gtzpnfnesk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.haohaochexian.top/gtfcgxezng.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtxvyswxxm.html

Ruby: return a, b
来源：http://hz.tian-w.cn/gtqzqemcqu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.svipenyu.cn/gtrukazjse.html


<!-- 参考信息 -->