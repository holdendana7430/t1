代发 wailian999

[A14] 注释写法
来源：http://hz.shzxlz.cn/gtzdpaugve.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.andypj.xyz/gtrxlaqcgg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.aibaodan.cn/gtdnbxhkto.html

JS:   // 单行；/* 多行 */
来源：http://hz.nanxinkj.top/gtbzvzgmqs.html

TS:   // 单行；/* 多行 */
来源：http://hz.52xcode.cn/gticdeltwc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.shuidangran.top/gtrkkqxahd.html

Go:   // 单行；/* 多行 */
来源：http://hz.chenzaomai.com/gtommiumyd.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ppjwa.cn/gtwdiglhlt.html

C#:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtzbkmqnej.html

[A15] 空值判断与默认值
来源：http://hz.dianchejie.cn/gtckvkpfan.html

Py:   value = data or "默认值"
来源：http://hz.ywan-chungtsiang.top/gtfyrzzntd.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jqgfzy.top/gtstomrprj.html

JS:   const value = data ?? "默认值";
来源：http://hz.sysykeji.top/gtswgbxjct.html

TS:   const value = data ?? "默认值";
来源：http://hz.sufxvd.cn/gtgajpylka.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.sufxvd.cn/gthmkqtynw.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jinqigufen.top/gthxfwmikr.html

Ruby: value = data || "默认值"
来源：http://hz.yj202588.top/gtkjwvmqsf.html

C#:   var value = data ?? "默认值";
来源：http://hz.yvedp.cn/gtkksfrrpa.html

[A16] 真假值判断规则
来源：http://hz.aibaodan.cn/gtwhjgpwqh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.dianchejie.cn/gtctxrzqnm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.snrcjt.cn/gtamccxuqa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yj20258.top/gtslkepobd.html

TS:   if (!x) {}
来源：http://hz.jinghuilouyu.cn/gtkxujncnu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yonumen.top/gtcrmzrxrs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.guannengcc.top/gtniawitwh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.daria6918.cn/gtbbxfjhfg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.kuanghao11.cn/gtcpttnajb.html

[A17] 位运算
来源：http://hz.sweek.top/gtcuzeqgpg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtxfhejiuh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhongyouzk.top/gttjrkarsf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gtaksbgnne.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtgwsnnpca.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtjhmlspso.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtsmtcfnuj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtagnwghyb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gteobpoiln.html

[A18] 字符与 ASCII 码互转
来源：http://hz.xuetiantiany.cn/gtakblzwgo.html

Py:   ord("A"); chr(65)
来源：http://hz.cheryme.top/gtymjsjrnd.html

PHP:  ord("A"); chr(65)
来源：http://hz.cheryme.top/gtslvpdgkb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sufxvd.cn/gtqdjikjdv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.fengsongda.top/gtgsffkwea.html

Java: (int) 'A'; (char) 65
来源：http://hz.iojbl.cn/gtyzbyowgu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jlsjyb.cn/gtixeofmwh.html

Ruby: "A".ord; 65.chr
来源：http://hz.hongshengwenyu.top/gtblbasrdw.html

C#:   (int)'A'; (char)65
来源：http://hz.hfpthk.cn/gtnijfxpkp.html

[A19] 交换两个变量
来源：http://hz.fzhhl.top/gtmlgfbzol.html

Py:   a, b = b, a
来源：http://hz.zhixingplan.top/gthzwbdpsh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.cdnleiting.top/gtujcncmxu.html

JS:   [a, b] = [b, a];
来源：http://hz.shuidangran.top/gtwvqavpeh.html

TS:   [a, b] = [b, a];
来源：http://hz.jqgufenzy.top/gtabwhgqvc.html

Java: int t = a; a = b; b = t;
来源：http://hz.nanxuanxn.top/gtauupzsqg.html

Go:   a, b = b, a
来源：http://hz.daxiang520.top/gtfrvolydy.html

Ruby: a, b = b, a
来源：http://hz.yj20258.top/gtgokwbsad.html

C#:   (a, b) = (b, a);
来源：http://hz.yj20258888.top/gtfpniyeot.html

[A20] 读取标准输入
来源：http://hz.nanxuanxn.top/gtdomfnswo.html

Py:   name = input("请输入：")
来源：http://hz.yanxiufei.cn/gtwgvxupxl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.shanyushiyangkeji.top/gtzwoqvadu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.smart0.xyz/gtwhisgkfr.html

TS:   // Node.js：readline 模块
来源：http://hz.jinqigufen.top/gticiizgoq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.shanyushiyangkeji.top/gtugwwpueb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhongyouzk.top/gttbnmmrac.html

Ruby: gets.chomp
来源：http://hz.yangfankeji.com/gtgfdwngku.html

C#:   Console.ReadLine();
来源：http://hz.yj202588.top/gtzdsevjqk.html

[A21] 保留指定小数位输出
来源：http://hz.zdqjudy.top/gthumaqzhm.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zhijiandao.cn/gtxyqlcbnh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.andypj.xyz/gtxgdtvprv.html

JS:   (3.14159).toFixed(2)
来源：http://hz.nwbrower.top/gtnubnnxua.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yj20258888.top/gtoabeicnt.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinghuilouyu.cn/gtouauysri.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gtcedeeplw.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.nanxuanxn.top/gtytlpsfzk.html

C#:   3.14159.ToString("F2")
来源：http://hz.pycfn.com/gtqspkgnfc.html

[A22] 获取字符串长度
来源：http://hz.smart0.xyz/gtkfkftrok.html

Py:   len(s)
来源：http://hz.shangyingyoupin.top/gtddcgawng.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.tanke756.top/gtztwuypep.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.shangyingyoupin.top/gtzggjefhc.html

TS:   s.length
来源：http://hz.gotoacloud.top/gtoxlapzmr.html

Java: s.length()
来源：http://hz.haohaochexian.top/gtjwtkqbey.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.daria6918.cn/gtvoykihpt.html

Ruby: s.length
来源：http://hz.hnxiangtu.top/gtfjxqonfj.html

C#:   s.Length
来源：http://hz.sufxvd.cn/gtzfytsrkm.html

[A23] 大小写转换
来源：http://hz.guowangkeji.top/gtpjhsykrf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.bjfxy.top/gtuqbbhgyn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.jianghu66.top/gtegpkvzgx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.aibaodan.cn/gtlcayypny.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.nwbrower.top/gthocghgqf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhengqikj.top/gtveuitefa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yuanzhike.top/gtuidbdega.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuetiantiany.cn/gtxfajcogp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.haohaochexian.top/gtznrnjntj.html

[A24] 去除首尾空白
来源：http://hz.316326.xyz/gtkczpehpj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yuxming.cn/gthewamxct.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jyoumei.cn/gtupefodsc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shangyingyoupin.top/gtlygqguai.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gaohongyu789.top/gtfzqexxha.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yonumen.top/gtsvryifkb.html

Go:   strings.TrimSpace(s)
来源：http://hz.dianchejie.cn/gtflecfkct.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.chenzaomai.com/gtcnevjatt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cqqwz.cn/gtygsdhovq.html

[A25] 字符串比较
来源：http://hz.gotoacloud.top/gtbqfxwnhf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ywan-chungtsiang.top/gtvcentzbh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.andypj.xyz/gtvyogjyxo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.birdmap.top/gtrbruinzf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.birdmap.top/gtimhkacqe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tianlin.xyz/gtgvfzrwpg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.tianlin.xyz/gttncdfjlp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yj20258888.top/gthrzspzua.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gotoacloud.top/gtdrljmqtl.html

[A26] 类型转换总览
来源：http://hz.aizwys.cn/gtopguehjz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.aizwys.cn/gthdufjbmm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zdqjudy.top/gtwvtxjpft.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xziqi.cn/gtudroyehk.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhixingplan.top/gtcgiwqnkh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ehwqpu.com/gtjuqktpae.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.wangdashe.top/gtmfksaabj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hammf.cn/gtajapwxqh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.pengpengdd.cyou/gtkrfojsmo.html

================================================================================
来源：http://hz.xziqi.cn/gtrieoparj.html

B. 流程控制
来源：http://hz.xingfuxueyuan.xyz/gtrcjztmma.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyxuztybf.html

[B01] 条件判断 if / else
来源：http://hz.chenjidiqi.icu/gtlkmnwhzh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yanxiufei.cn/gtsiwbgloq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.birdmap.top/gtrqbmufkc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hysaishi.cn/gtcypfhjws.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nwbrower.top/gtjwgtyolk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtrzqtylnt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hywenlv.cn/gtcwcrcmoj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shuidangran.top/gtzrvxszux.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtahlakahz.html

[B02] 多分支 else if / elif
来源：http://hz.yonumen.top/gtvjfevnjs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.dashuyun.cn/gtwzmipueo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.nanxinkj.top/gtalshccrg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gtwvgasiri.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gttpbotsnh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtpggttolp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.aibaodan.cn/gtvssrwfbg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.haohaochexian.top/gtpdngebzo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gtkensfijm.html

[B03] switch / match / case
来源：http://hz.gaohongyu789.top/gtoxwzltdb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258888.top/gtofboagjm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hnqzz.top/gtfmnfkuzt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hywenlv.cn/gtpqtvrekr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yuanzhike.top/gtxmvogvxa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.haohaochexian.top/gtzywclyoc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ydzc1.top/gtppfkvbhb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.guowangkeji.top/gtcxpwnzhl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hysaishi.cn/gtifkvufkd.html

[B04] for 计数循环
来源：http://hz.xylfe.cn/gtyaxiccwp.html

Py:   for i in range(10): print(i)
来源：http://hz.cucudq.cn/gtanfizjvy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.chenjidiqi.icu/gtkzsmqoxk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sxryk.cn/gtahsklupj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.smart0.xyz/gtfmwsweck.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinghuilouyu.cn/gtlfaxaons.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.gaohongyu789.top/gtuhqlmbra.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yvedp.cn/gtzahttrku.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hnqzz.top/gtlcxxvqry.html

[B05] 遍历数组 / 列表
来源：http://hz.hfpthk.cn/gttleoaphl.html

Py:   for item in arr: print(item)
来源：http://hz.cheryme.top/gtcmnbopse.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yuxming.cn/gtgwpafeku.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yonumen.top/gtedhfuxcn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.316326.xyz/gtaszlbpac.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.kuanghao11.cn/gtmlkghrwq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhixingplan.top/gtvwexwjys.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhaomingkeji.xyz/gtxnrfshzu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.haohaochexian.top/gthtahasek.html

[B06] 遍历字典 / 对象
来源：http://hz.shuidangran.top/gtvktsyihv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.andypj.xyz/gtgmnchyvk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gaohongyu789.top/gtvtvoaqrc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ehwqpu.com/gthsscbfts.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sysykeji.top/gtdxtljjhz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sweek.top/gtdzfogkaj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhoulong.xyz/gtwwonzmik.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xingfuxueyuan.xyz/gtgvdoqelq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.daria6918.cn/gtnbrpqidz.html

[B07] while 循环
来源：http://hz.redwolf501.top/gtaxjibfgj.html

Py:   while i < 10: i += 1
来源：http://hz.hfpthk.cn/gtpbajtfrf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.52xcode.cn/gtbayjymin.html

JS:   while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gtkvtqcthl.html

TS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtbddjhoow.html

Java: while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtzzaszzvr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangdashe.top/gtwgpglsra.html

Ruby: while i < 10; i += 1; end
来源：http://hz.snrcjt.cn/gtsmvhcjie.html

C#:   while (i < 10) { i++; }
来源：http://hz.shzxlz.cn/gtfnmjlfjy.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258888.top/gtcjjzhvpz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gtzlzmbgyv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hfpthk.cn/gtykyvgaod.html

JS:   do { i++; } while (i < 10);
来源：http://hz.wangshuangyany.cn/gtstfrsezc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtsaldyxfb.html

Java: do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtvmfpiwnv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhixingplan.top/gtyqcvrtvv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hysaishi.cn/gtcjhgqokt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtzzzstzeq.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gtpxtdlbxt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.smart0.xyz/gtckeuwdxu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.chenzaomai.com/gtxihsdyfl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fengsongda.top/gtahlgeojr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtjqxdclna.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zycfv.cn/gtleenvqhq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gthzsnefwz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtixiytxzg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gthhgszbeu.html

[B10] 遍历同时拿索引
来源：http://hz.tian-w.cn/gtxlfyvvor.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtvsldzjbt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cheryme.top/gtpbfjivtc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtkgxsyahi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tian-w.cn/gtqmmibpwv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.c1oappe.top/gtjonllhfo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hysaishi.cn/gtuxqiyyyr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangdashe.top/gtpmxgymxe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jiagoushi.top/gtakgyxubn.html

[B11] 生成数字序列 / 区间
来源：http://hz.ywan-chungtsiang.top/gtottqbawk.html

Py:   list(range(0, 10, 2))
来源：http://hz.xziqi.cn/gteiasnlwc.html

PHP:  range(0, 10, 2);
来源：http://hz.jinyuanbaomall.cn/gtsuwxdgfp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gtkqrgoozo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.9152youxi.cn/gthhsrxqyl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtvktohknj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ydjk.org.cn/gtkoyadstj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jiagoushi.top/gtgyveadiq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ybcxt.top/gtzhlecmqi.html

[B12] 跳出多层循环
来源：http://hz.52xcode.cn/gtovmawlnk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhixingplan.top/gtmjobvwdk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.mhx1999.top/gtvcoskico.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtbngqsxxb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtzmvpjxps.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtabcftvsi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gaohongyu789.top/gtjnivwmes.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guannengcc.top/gtcokdqidg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xuetiantiany.cn/gthpmobysp.html

[B13] 判断是否为数字
来源：http://hz.shzxlz.cn/gtugjpyjep.html

Py:   isinstance(x, (int, float))
来源：http://hz.wangshuangyany.cn/gtmftwletn.html

PHP:  is_numeric($x)
来源：http://hz.hnxiangtu.top/gthmredpoi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtiqosnynh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zycfv.cn/gtzttfeets.html

Java: x instanceof Number
来源：http://hz.ywan-chungtsiang.top/gtwfbjhtec.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cucudq.cn/gtajhvwiot.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxuanxn.top/gtyqkrevoz.html

C#:   x is int or double or decimal
来源：http://hz.zhixingplan.top/gtgzkfwnqw.html

[B14] 判断值是否在集合内
来源：http://hz.9152youxi.cn/gtlqxggjun.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.bjfxy.top/gtumgkevyb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.vqdsnc.cn/gttehxpyou.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xuanzx.com/gtfsmfsgnb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtzvcdzipa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zycfv.cn/gtygudvait.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.iojbl.cn/gtvstlvxxv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yongpay.top/gtnroiifvn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gtlkocaivs.html

[B15] 布尔运算与取反
来源：http://hz.nanxuanxn.top/gtkpjuwvdu.html

Py:   a and b or not c
来源：http://hz.cdnleiting.top/gtijbdvwtx.html

PHP:  $a && $b || !$c
来源：http://hz.cheryme.top/gtwnlyapmy.html

JS:   a && b || !c
来源：http://hz.sufxvd.cn/gtmphlbqtm.html

TS:   a && b || !c
来源：http://hz.jqgfzy.top/gtfcpklegb.html

Java: a && b || !c
来源：http://hz.meibo888.top/gtzvummghm.html

Go:   a && b || !c
来源：http://hz.fengsongda.top/gtnntxxsdd.html

Ruby: a && b || !c
来源：http://hz.snrcjt.cn/gtddqbgedf.html

C#:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtxvgjerrr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sweek.top/gtfpnijcfg.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gtgeghwepw.html

PHP:  if (!$data) { return; }
来源：http://hz.shuidangran.top/gtzavnkjkd.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtazoyhgsg.html

TS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtdigweroa.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtlhdxdtxa.html

Go:   if data == nil { return }
来源：http://hz.yvedp.cn/gtoevapbzm.html

Ruby: return if data.nil?
来源：http://hz.yangfankeji.com/gtsehtsgza.html

C#:   if (data == null) return;
来源：http://hz.wangdashe.top/gtlckypiup.html

================================================================================
来源：http://hz.cdnleiting.top/gtlhsihvez.html

C. 函数与作用域
来源：http://hz.yueranfly.top/gtvlqmcqvt.html

================================================================================
来源：http://hz.fengsongda.top/gtznpnrkxu.html

[C01] 定义函数
来源：http://hz.andypj.xyz/gtwuahhcut.html

Py:   def add(a, b): return a + b
来源：http://hz.bjfxy.top/gttlwyhsae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtwpezjzzf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtydcknvwr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtidlaknyt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtcmxmvnbd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yanxiufei.cn/gthzskpwfb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.mhx1999.top/gtypzesudm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ivvv.top/gtbzqywgss.html

[C02] 默认参数
来源：http://hz.yonumen.top/gtjaorzimk.html

Py:   def greet(name="World"): return name
来源：http://hz.yongpay.top/gtssapedlu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.c1oappe.top/gtrjepqxpw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtapxpbuzd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cucudq.cn/gtskpdjeqv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj20258888.top/gtvrtdrafl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtkrvntdaw.html

Ruby: def greet(name = "World") = name
来源：http://hz.daria6918.cn/gtgsziqyhb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gtithykpou.html

[C03] 可变参数
来源：http://hz.redwolf501.top/gthafpotaf.html

Py:   def total(*args): return sum(args)
来源：http://hz.shangyingyoupin.top/gtkdfpefmq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258.top/gtoduwuwyh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtrzqrczjw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtqmtyhrpz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jiagoushi.top/gtvqkxsqrr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yvedp.cn/gtfarnbgyy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aizwys.cn/gtoancjtly.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhengqikj.top/gtithyxrjk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shzxlz.cn/gtqzisvnta.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zdqjudy.top/gtekqawpso.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jianghu66.top/gtahsfabrl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtpqbbrpxd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.kuanghao11.cn/gteawxawqw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yangfankeji.com/gtenpchisl.html


<!-- 参考信息 -->