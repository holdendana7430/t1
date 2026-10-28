代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.316326.xyz/gtxghqojiv.html

TS:   const value = data ?? "默认值";
来源：http://hz.pengpengdd.cyou/gtmqbpjmnn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shanyushiyangkeji.top/gtiejvngxf.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zhoulong.xyz/gtbgzzhvrn.html

Ruby: value = data || "默认值"
来源：http://hz.nanxinkj.top/gtycdpcaoc.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinqigfzy.top/gtjnsispkb.html

[A16] 真假值判断规则
来源：http://hz.fzhhl.top/gtywhwogob.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.sufxvd.cn/gtbtsawwau.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.ppjwa.cn/gtzqojomcj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jlsjyb.cn/gtcgxqvbin.html

TS:   if (!x) {}
来源：http://hz.jqgufenzy.top/gtfhjdhsue.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.zhaomingkeji.xyz/gtpxdainge.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhiwuduotai.top/gthgguqqbs.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.xinyue.icu/gthpdjwntf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.aibaodan.cn/gtiesxhman.html

[A17] 位运算
来源：http://hz.haohaochexian.top/gtqaalgsvl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtquqyvtek.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.redwolf501.top/gtbdizfdqu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.52xcode.cn/gteexiyfav.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gtereqajtj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtlpvtjxma.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.bjfxy.top/gtcouzdbbl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtwkxcaaer.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jqgufenzy.top/gtslvynjbs.html

[A18] 字符与 ASCII 码互转
来源：http://hz.iojbl.cn/gtxwovbmwr.html

Py:   ord("A"); chr(65)
来源：http://hz.cqqwz.cn/gtuylhqpln.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhijiandao.cn/gtexaowabe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yj20258.top/gtayodplee.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zdqjudy.top/gtzngzsgep.html

Java: (int) 'A'; (char) 65
来源：http://hz.yuanzhike.top/gtaoxjnjzr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.ivvv.top/gtsewewmcs.html

Ruby: "A".ord; 65.chr
来源：http://hz.chenzaomai.com/gtidocbbiu.html

C#:   (int)'A'; (char)65
来源：http://hz.shangyingyoupin.top/gtiukdqqaj.html

[A19] 交换两个变量
来源：http://hz.ydzc1.top/gtxpsfpmgu.html

Py:   a, b = b, a
来源：http://hz.chenlongwang.top/gtoulmtzdq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shanyushiyangtech.top/gtjnphnujb.html

JS:   [a, b] = [b, a];
来源：http://hz.daria6918.cn/gtgtucoteb.html

TS:   [a, b] = [b, a];
来源：http://hz.hnxiangtu.top/gthvliariz.html

Java: int t = a; a = b; b = t;
来源：http://hz.hywenlv.cn/gtoqojirge.html

Go:   a, b = b, a
来源：http://hz.chenzaomai.com/gtwtjooaut.html

Ruby: a, b = b, a
来源：http://hz.hnqzz.top/gtopujlzxe.html

C#:   (a, b) = (b, a);
来源：http://hz.cashguo.top/gtcjxdvkgv.html

[A20] 读取标准输入
来源：http://hz.fzhhl.top/gtzivdwuhq.html

Py:   name = input("请输入：")
来源：http://hz.redwolf501.top/gtuazmdgvy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yangfankeji.com/gtjuhcszqc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shanyushiyangkeji.top/gtsqrzgyfu.html

TS:   // Node.js：readline 模块
来源：http://hz.shzxlz.cn/gtkfmvfywm.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhijiandao.cn/gtnrsulzvf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ppjwa.cn/gtftqrjgnj.html

Ruby: gets.chomp
来源：http://hz.andypj.xyz/gtimxnddzq.html

C#:   Console.ReadLine();
来源：http://hz.shanyushiyangkeji.top/gtfwcxbymx.html

[A21] 保留指定小数位输出
来源：http://hz.zhaomingkeji.xyz/gtplzdyotw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ydzc1.top/gtjrsjbuuj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.iojbl.cn/gtkfmzhydq.html

JS:   (3.14159).toFixed(2)
来源：http://hz.fengsongda.top/gterhseopq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.smart0.xyz/gtamlapjaf.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.guannengcc.top/gtzvpzagol.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtsrnncmuq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtozfqhxza.html

C#:   3.14159.ToString("F2")
来源：http://hz.chenjidiqi.icu/gtyccbywnm.html

[A22] 获取字符串长度
来源：http://hz.xylfe.cn/gtxfwitcek.html

Py:   len(s)
来源：http://hz.feifeiyinyue.top/gtzgyubfyf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xuetiantiany.cn/gtrsrgbhas.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yonumen.top/gtutvxaefj.html

TS:   s.length
来源：http://hz.yueranfly.top/gtlekestct.html

Java: s.length()
来源：http://hz.9152youxi.cn/gtkwmlozvu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.shuidangran.top/gtsdrjtdlu.html

Ruby: s.length
来源：http://hz.yuanzhike.top/gtiswlilrk.html

C#:   s.Length
来源：http://hz.andypj.xyz/gttcjveqgv.html

[A23] 大小写转换
来源：http://hz.xylfe.cn/gtkdooqnrg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tianlin.xyz/gtechmxfgs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhixingplan.top/gtpdnzkzcf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangtech.top/gtkywkossb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtvomftmso.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jiagoushi.top/gtxzpsagwt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zdqjudy.top/gtjpukgsnv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xziqi.cn/gtepjkofoz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gaohongyu789.top/gtiecvwwja.html

[A24] 去除首尾空白
来源：http://hz.zhengqikj.top/gtjhdlmuma.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jinqigfzy.top/gtlqktozdj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xinyue.icu/gtdhaijbbc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigufen.top/gtohrdrghv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhixingplan.top/gtzdwskgyy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.pengpengdd.cyou/gthgtysnvb.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhongyouzk.top/gtwabauqno.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.wangdashe.top/gttscevsqy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yuxming.cn/gtyqzwrtpi.html

[A25] 字符串比较
来源：http://hz.yj20258888.top/gtitxyspgs.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinghuilouyu.cn/gtpgljwyao.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yj20258.top/gthxgxhhio.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sysykeji.top/gttpameorm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hfpthk.cn/gtegubxqya.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hongshengwenyu.top/gtvbqjnfen.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yueranfly.top/gtgpruqwbp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hnqzz.top/gtjmcbygcj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xuetiantiany.cn/gtureinfux.html

[A26] 类型转换总览
来源：http://hz.chenjidiqi.icu/gtagfdaudl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.wangshuangyany.cn/gtcrcctqfz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yj202588.top/gtwhdpzzxb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zdqjudy.top/gttmpkrdzu.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yonumen.top/gtwzudxgev.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenlongwang.top/gtansgaydk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhengqikj.top/gtajkkjqha.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hywenlv.cn/gtbbaaurmw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xinyue.icu/gtkfiydbgx.html

================================================================================
来源：http://hz.0kj1m.cn/gtqdhotgdd.html

B. 流程控制
来源：http://hz.hfpthk.cn/gtphscpbze.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtosglolmd.html

[B01] 条件判断 if / else
来源：http://hz.svipenyu.cn/gtjivvwutt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.chenlongwang.top/gtdbwkbezr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jlsjyb.cn/gtrufbnbcj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtajupvssk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ydzc1.top/gtnespsetz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtdzxfkwuh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.mhx1999.top/gtworlfofs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.fzhhl.top/gtgqthjlbs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtkufazkvc.html

[B02] 多分支 else if / elif
来源：http://hz.nanxinkj.top/gtuestcxku.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhixingplan.top/gtsosafcmb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yvedp.cn/gtuomrsqcr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gtuckjspgk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtbpbloton.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gtvaahidcv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.birdmap.top/gtkhgbowar.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hongshengwenyu.top/gtqbeendal.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtfhcvdbyv.html

[B03] switch / match / case
来源：http://hz.iojbl.cn/gtvobscnol.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.c1oappe.top/gttxqnhtfs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ybcxt.top/gtmdruzlfg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hfpthk.cn/gtimfirmcf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yonumen.top/gtociolnsh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenzaomai.com/gtlozrqmel.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.dashuyun.cn/gtpyxryiwx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cucudq.cn/gtyxwcjdso.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ehwqpu.com/gtasuvsghc.html

[B04] for 计数循环
来源：http://hz.chenzaomai.com/gtpfrbqxje.html

Py:   for i in range(10): print(i)
来源：http://hz.chenjidiqi.icu/gtyygtdfeu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jlsjyb.cn/gtmsyzgjwv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtcmfuebhm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.redwolf501.top/gteggkygoj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yuxming.cn/gtpzahrrhm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.birdmap.top/gtufqpnpnd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shanyushiyangtech.top/gtsoieboiw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ydjk.org.cn/gtvabvaxkm.html

[B05] 遍历数组 / 列表
来源：http://hz.gaohongyu789.top/gtrthjfcaj.html

Py:   for item in arr: print(item)
来源：http://hz.tianlin.xyz/gtrhocyvvr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xingfuxueyuan.xyz/gtyweijqpe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.meibo888.top/gtzsxvxnxx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.nanxinkj.top/gtuwpmzfpw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jlsjyb.cn/gtuflayqmk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shanyushiyangkeji.top/gtwvtvcceb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.andypj.xyz/gtkmfoaotj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yonumen.top/gtaknrtexa.html

[B06] 遍历字典 / 对象
来源：http://hz.xingfuxueyuan.xyz/gtbyntdfud.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xuanzx.com/gtbzgnuvpv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.0kj1m.cn/gtgbtgfdxb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhongyouzk.top/gtzudoxuhf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ppjwa.cn/gtcurzpdsy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhoulong.xyz/gtmsopcihe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangshuangyany.cn/gtamolikxl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.daria6918.cn/gtltzjbnzu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jiagoushi.top/gttrabbyht.html

[B07] while 循环
来源：http://hz.ybcxt.top/gtkxtyzlzx.html

Py:   while i < 10: i += 1
来源：http://hz.zhiwuduotai.top/gtxmyyjuxk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yj20258888.top/gtpdabfxyi.html

JS:   while (i < 10) { i++; }
来源：http://hz.sweek.top/gthursuwds.html

TS:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtbvhmbglr.html

Java: while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtaqxdrivn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cdnleiting.top/gtxgdbytoc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.c1oappe.top/gtrnxnesds.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtutiksezt.html

[B08] do-while（至少执行一次）
来源：http://hz.pengpengdd.cyou/gtxzgyofoo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.dashuyun.cn/gteuqkbzdk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gtuvqsdcmp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtckjfjueg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtbsgkaezo.html

Java: do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gthcilmhjl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gotoacloud.top/gtitzmpdtr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.316326.xyz/gtfpiudegz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtrwtmfllq.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gtmoailowe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tian-w.cn/gtyenadcpk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nanxuanxn.top/gtughjxdbq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtoatsmske.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtuqvvsoja.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtajpofjmb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hywenlv.cn/gtxvuilsvk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.smart0.xyz/gtfwfqemsz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtwwzzvvks.html

[B10] 遍历同时拿索引
来源：http://hz.sysykeji.top/gtzpppkjhg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj202588.top/gtzmanwdkl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ehwqpu.com/gtlyynsexe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtwdevnoxw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinghuilouyu.cn/gtcuxsbuli.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.meibo888.top/gteytjrgme.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aizwys.cn/gtvymnfxgx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258888.top/gtesjexvqe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dianchejie.cn/gtxjkcponj.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gtjkdamjsg.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtyiddpzin.html

PHP:  range(0, 10, 2);
来源：http://hz.birdmap.top/gttelycbvf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnqzz.top/gtcbehnjjh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtuhhejczt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gzhubu.top/gtmbxwfidp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xziqi.cn/gtlpsrjcze.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sweek.top/gtxhcanwbj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cashguo.top/gtzbwkqfno.html

[B12] 跳出多层循环
来源：http://hz.guowangkeji.top/gtzmypnbcw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ywan-chungtsiang.top/gteozeqehy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenjidiqi.icu/gtiviszbcx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gttsmcrxtx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtjqwkbtvm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtigurgbct.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gtbiugdrmg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shanyushiyangtech.top/gttlcgiisp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.svipenyu.cn/gtqzjwxahw.html

[B13] 判断是否为数字
来源：http://hz.vqdsnc.cn/gtzpynfvco.html

Py:   isinstance(x, (int, float))
来源：http://hz.kuanghao11.cn/gtvlftrseu.html

PHP:  is_numeric($x)
来源：http://hz.hnxiangtu.top/gtrysrmqlh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.feifeiyinyue.top/gtcjnqiggz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xingfuxueyuan.xyz/gtltgpqmah.html

Java: x instanceof Number
来源：http://hz.zhixingplan.top/gtsgzowsho.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangdashe.top/gtqakuicsy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zycfv.cn/gtycqeearp.html

C#:   x is int or double or decimal
来源：http://hz.quarkkingdee.top/gttbicebpt.html

[B14] 判断值是否在集合内
来源：http://hz.ywan-chungtsiang.top/gtyshmzsfc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhoulong.xyz/gtqzibzteq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yuanzhike.top/gtmbjeyorq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.fzhhl.top/gtbqaurxcq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtesbtlqhg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dianchejie.cn/gtdakqdbbm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.haohaochexian.top/gtoryzylcd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pengpengdd.cyou/gtxzwixlgp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hysaishi.cn/gtqmsscdkn.html

[B15] 布尔运算与取反
来源：http://hz.xylfe.cn/gtalctyxwl.html

Py:   a and b or not c
来源：http://hz.quarkkingdee.top/gtqpmvzggy.html

PHP:  $a && $b || !$c
来源：http://hz.meibo888.top/gtwdomnkmc.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtbqfpccvq.html

TS:   a && b || !c
来源：http://hz.nwbrower.top/gtlsgexhsf.html

Java: a && b || !c
来源：http://hz.vqdsnc.cn/gtwlhuavrv.html

Go:   a && b || !c
来源：http://hz.cashguo.top/gtrtjprxhi.html

Ruby: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtzlllewnt.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gtytogbrnf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yueranfly.top/gtefdxiuzg.html

Py:   if not data: return
来源：http://hz.hnxiangtu.top/gtcnhvzwxm.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtkitjnfpd.html

JS:   if (!data) return;
来源：http://hz.pycfn.com/gtyfeufrlk.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtkfazlrgw.html

Java: if (data == null) return;
来源：http://hz.sxryk.cn/gteiqnkyay.html

Go:   if data == nil { return }
来源：http://hz.zhiwuduotai.top/gtsatiomlq.html

Ruby: return if data.nil?
来源：http://hz.xinyue.icu/gtqmxkoiwx.html

C#:   if (data == null) return;
来源：http://hz.yj202588.top/gtoorzqmiz.html

================================================================================
来源：http://hz.yangfankeji.com/gttnxmdcdl.html

C. 函数与作用域
来源：http://hz.zhiwuduotai.top/gtxuhhzvfw.html

================================================================================
来源：http://hz.yj20258888.top/gtbbxcagvo.html

[C01] 定义函数
来源：http://hz.zhiwuduotai.top/gtkvsyvjsp.html

Py:   def add(a, b): return a + b
来源：http://hz.shzxlz.cn/gtyrsotrdq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtuvwowzvg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtfqqqwuvi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtljqyaajz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtbycxsiiz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtioxzzrsm.html

Ruby: def add(a, b); a + b; end
来源：http://hz.birdmap.top/gtqsgdtnjr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtkkkjfaiz.html

[C02] 默认参数
来源：http://hz.ydzc1.top/gthvwzvshu.html

Py:   def greet(name="World"): return name
来源：http://hz.yanxiufei.cn/gtctwshrhx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shuidangran.top/gtapztjfyp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtolkbndwu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtqtdrqeit.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhengqikj.top/gtepgecwgq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxinkj.top/gtbjawepkv.html

Ruby: def greet(name = "World") = name
来源：http://hz.guowangkeji.top/gtairjrffq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hysaishi.cn/gtezxaumuv.html

[C03] 可变参数
来源：http://hz.bjfxy.top/gtyvqahymb.html

Py:   def total(*args): return sum(args)
来源：http://hz.cashguo.top/gtdjxdibnk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sysykeji.top/gtyamujbci.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtxtjgaryg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtplusxgnc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtzvbmsdlj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.316326.xyz/gtiakorwiz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hammf.cn/gtaklqvjpl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtufwuyqad.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gtglmupbbj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtlozhyehd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenzaomai.com/gtgqckkrws.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gtugyzibpb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigfzy.top/gtjdnvayse.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hysaishi.cn/gttqziimkv.html

Go:   // 无：用配置结构体参数
来源：http://hz.smart0.xyz/gthoyjfssu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtmimgfryu.html

C#:   f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtmjdvuanu.html

[C05] 返回多个值
来源：http://hz.daria6918.cn/gtokangodc.html

Py:   return a, b
来源：http://hz.guannengcc.top/gtqfyojetv.html

PHP:  return [$a, $b];
来源：http://hz.nanxuanxn.top/gtvsuojzlt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ppjwa.cn/gtmrtbybfl.html

TS:   return { a, b };
来源：http://hz.guannengcc.top/gturuirkyb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gogol.net.cn/gtmjzdbjja.html

Go:   return a, b
来源：http://hz.tanke756.top/gtdukdites.html

Ruby: return a, b
来源：http://hz.cashguo.top/gtcnsjtkyr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258888.top/gtrscqmzuz.html


<!-- 参考信息 -->