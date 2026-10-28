代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtypinpiox.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sysykeji.top/gtjxqlaiyj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gtsntujvwb.html

C#:   new List<int>(list);
来源：http://hz.svipenyu.cn/gtfzixoaya.html

[D23] reduce 累积计算
来源：http://hz.xziqi.cn/gtdpivyakk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhaomingkeji.xyz/gtpragmmhq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuxming.cn/gtnisvcyru.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtwmjwawrz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtrhuxehpc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cashguo.top/gtlwsusifb.html

Go:   // 手写循环
来源：http://hz.hnxiangtu.top/gtsifuaauh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnxiangtu.top/gtypleaonw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258.top/gtugyilfec.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gtbkkceuyy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shangyingyoupin.top/gtfdmvpjjp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtxpnnjroi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jlsjyb.cn/gtyfqwfrph.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.dashuyun.cn/gtnfsjyzad.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nwbrower.top/gtskovqsge.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tianlin.xyz/gtyulwiuik.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dianchejie.cn/gtmrpzodjt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pycfn.com/gtlbopnhct.html

[D25] Set 集合去重与交并差
来源：http://hz.hysaishi.cn/gtxlstcwyq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.birdmap.top/gtbwjdtizr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtsunqnwae.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dashuyun.cn/gtuapqcjvm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sxryk.cn/gtroydvzea.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cqqwz.cn/gtionunabd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtamjduyxc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aizwys.cn/gtgdqvnndd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtcfqvklfu.html

[D26] 数组转字符串
来源：http://hz.daria6918.cn/gtpxnidjny.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtasuxrqrx.html

PHP:  implode(", ", $arr);
来源：http://hz.yonumen.top/gtwdvkptqk.html

JS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gttxgjrvwf.html

TS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtghyqcrty.html

Java: String.join(", ", list)
来源：http://hz.shzxlz.cn/gtzexkkcmj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtlwszwimu.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtkaktkyzq.html

C#:   string.Join(", ", list)
来源：http://hz.hongshengwenyu.top/gtublphrcr.html

================================================================================
来源：http://hz.haohaochexian.top/gtqbhwvylt.html

E. 字符串处理
来源：http://hz.dashuyun.cn/gtupgwmtni.html

================================================================================
来源：http://hz.52xcode.cn/gtpxhuuucq.html

[E01] 拼接字符串
来源：http://hz.yj202588.top/gtmefjjvnk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hywenlv.cn/gtlvgudwrj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtxuccjzgi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gthkvxsbqa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtgiqkwscg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtktutbnep.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.c1oappe.top/gtkzocrtnt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnxiangtu.top/gtysnzrvfj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.andypj.xyz/gtzvxcfmhr.html

[E02] 重复字符串
来源：http://hz.shanyushiyangtech.top/gtsajnvufv.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtqibegxum.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhixingplan.top/gtccrfsdsv.html

JS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtrkntqjws.html

TS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtnjceoxpu.html

Java: "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtehyuyhud.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtgqwlckux.html

Ruby: "ab" * 3
来源：http://hz.dianchejie.cn/gteynytkvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnqzz.top/gttvioaxqt.html

[E03] 截取子串
来源：http://hz.xziqi.cn/gtjvuppfnv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgufenzy.top/gtinmbtfvg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hysaishi.cn/gtqjijgboi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.mhx1999.top/gtorcpzvtc.html

TS:   s.slice(1, 4)
来源：http://hz.snrcjt.cn/gtkvdobulp.html

Java: s.substring(1, 4)
来源：http://hz.yj20258888.top/gtawemhpel.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guowangkeji.top/gttsmkbpyc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aibaodan.cn/gtjdohokxt.html

C#:   s.Substring(1, 3)
来源：http://hz.xuetiantiany.cn/gtlgszfhxr.html

[E04] 查找子串位置
来源：http://hz.zhaomingkeji.xyz/gtqwcivqyp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dianchejie.cn/gtptcgcjyj.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtlxucdfwy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xuanzx.com/gtybvhugih.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtapaxzxjv.html

Java: s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtayjekeby.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtqxinhqzx.html

Ruby: s.index("x")
来源：http://hz.yj20258.top/gtgxdilmcn.html

C#:   s.IndexOf("x")
来源：http://hz.zhixingplan.top/gtaxndlfiy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangshuangyany.cn/gtiswaaxeo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gotoacloud.top/gtrgyaxund.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtvbbtoawt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtwzpdcwbx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtkryfoaqx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtgkhfuhbj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.52xcode.cn/gtnzmrgvze.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangshuangyany.cn/gtjdrxcjgw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cheryme.top/gtpiwimccz.html

[E06] 替换子串
来源：http://hz.zhengqikj.top/gteuflvghn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtvmuimmrz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yongpay.top/gtmohhybkx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtvvafsldg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtebdlsurz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtswtmwsti.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yueranfly.top/gtqfyfpkli.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtqasxmpqo.html

C#:   s.Replace("a", "b")
来源：http://hz.gotoacloud.top/gtensyrfue.html

[E07] 按分隔符拆分
来源：http://hz.jianghu66.top/gtgxwnispz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ywan-chungtsiang.top/gtjhaamaud.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gtnadoplub.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gogol.net.cn/gtxlcyjmfe.html

TS:   s.split(",")
来源：http://hz.mhx1999.top/gtzlqzpoxl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xylfe.cn/gtlprzawfu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fzhhl.top/gtnplbqlww.html

Ruby: s.split(",");  s.split
来源：http://hz.hfpthk.cn/gtjbtzrqsr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.316326.xyz/gtnwwwgmrv.html

[E08] 数组按分隔符合并
来源：http://hz.andypj.xyz/gtrqekqddo.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtgzzwvdhj.html

PHP:  implode(",", $items);
来源：http://hz.tianlin.xyz/gtdmhhaykn.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtepxsdilg.html

TS:   items.join(",")
来源：http://hz.tanke756.top/gtruspqvpu.html

Java: String.join(",", items)
来源：http://hz.shuidangran.top/gtoxhwvppp.html

Go:   strings.Join(items, ",")
来源：http://hz.xinyue.icu/gtbzlbhbwb.html

Ruby: items.join(",")
来源：http://hz.pycfn.com/gtygyditbd.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gtnftnzmmk.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gthhsopxnf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtfpjrnpzo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.havefunace.top/gtunewkxsi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sxryk.cn/gthmfgyjbc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtssddzxhi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gturijwmnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tanke756.top/gttwxksnrl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuanzhike.top/gtdhtgykzk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.mhx1999.top/gtnjutjyim.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gotoacloud.top/gtalivyotq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxuanxn.top/gtgjxbaevt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cucudq.cn/gtrgzuokkp.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtwwgciqus.html

TS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtmcyonwnm.html

Java: String.format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtrrgmosfe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cdnleiting.top/gttmapojfs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.haohaochexian.top/gtyuwqmfho.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.iojbl.cn/gtcbepijte.html

[E11] 反转字符串
来源：http://hz.vqdsnc.cn/gtbhbsiaom.html

Py:   s[::-1]
来源：http://hz.redwolf501.top/gtgzsxerfl.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtomxexkyq.html

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtrhnkldlp.html

TS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtetjsmsrb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgfzy.top/gtdmudpiza.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtoatxzykb.html

Ruby: s.reverse
来源：http://hz.xziqi.cn/gtmadxsmkl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gtkmmnhrwa.html

[E12] 统计某字符出现次数
来源：http://hz.ybcxt.top/gtpwwhpiln.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtcdodjora.html

PHP:  substr_count($s, "a");
来源：http://hz.dianchejie.cn/gtiqkyekez.html

JS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtxemqxemo.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtzxutnkbl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.svipenyu.cn/gtkmgztfgc.html

Go:   strings.Count(s, "a")
来源：http://hz.shzxlz.cn/gtrnwsvjtc.html

Ruby: s.count("a")
来源：http://hz.jyoumei.cn/gtutlvfguf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.iojbl.cn/gtswtidxjj.html

[E13] 逐字符遍历
来源：http://hz.bjfxy.top/gtptegskqe.html

Py:   for ch in s: print(ch)
来源：http://hz.aizwys.cn/gtpernzrza.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gttqauiavu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtgjemylga.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtcpmawqoa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gogol.net.cn/gtroririxw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhiwuduotai.top/gtudirqxvx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sweek.top/gtgoxmgohb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gttpghgrcw.html

[E14] URL 编码与 Base64
来源：http://hz.yangfankeji.com/gtcsfnngnl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.meibo888.top/gttosnnhgd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenlongwang.top/gtaujpzmyi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtnhdvkjid.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigfzy.top/gteikwemkm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtvamllyvo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ehwqpu.com/gttpphcltn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.svipenyu.cn/gtvzirepiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hysaishi.cn/gtafacxleq.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtmmjgagui.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cashguo.top/gtmqjdcczn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xingfuxueyuan.xyz/gtqaizakup.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nanxuanxn.top/gtplnzbnta.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daxiang520.top/gtbjjqbwag.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.9152youxi.cn/gtgtuqmolh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.52xcode.cn/gtszrlhmwc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gtssupwbgn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daxiang520.top/gtsqveojqy.html

[E16] 数字千分位
来源：http://hz.nanxinkj.top/gtigetwipr.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangtech.top/gtlrguphln.html

PHP:  number_format(1234567);
来源：http://hz.jiagoushi.top/gtvwncosoh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtjqcphodg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gttucbmcqq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sysykeji.top/gtkhunlsld.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cucudq.cn/gtvtrjqlyx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtautovhpj.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gtnxppwnjx.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtkxdsieih.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gtopmkginv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yangfankeji.com/gtdmrptimh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtenfdmull.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtavxortll.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangshuangyany.cn/gtpvnulkfr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sxryk.cn/gtnkycapcu.html

Ruby: s.capitalize
来源：http://hz.hammf.cn/gtdxdwbmid.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhaomingkeji.xyz/gtektvusik.html

[E18] 模板占位符替换
来源：http://hz.shzxlz.cn/gtprwlqtnk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zycfv.cn/gtrpgrvtqa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.52xcode.cn/gtokcgthvg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtdqavknuz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtxmksjmkf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj202588.top/gtmhektilk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cqqwz.cn/gtompqpxaf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtnrgdywht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtnmmpfudj.html

[E19] 多行文本按行拆分
来源：http://hz.yanxiufei.cn/gtigfrnkzk.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtjxlwxkzr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxinkj.top/gtpbtnhtcq.html

JS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtgecemitl.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtipyvvtov.html

Java: s.lines().toList()
来源：http://hz.tian-w.cn/gtbyqmlhhi.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinghuilouyu.cn/gtslxjwlwl.html

Ruby: s.lines
来源：http://hz.sufxvd.cn/gtljmeognh.html

C#:   s.Split('\n')
来源：http://hz.daxiang520.top/gttwzalyes.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangtech.top/gtjdlvpluo.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gtiskbtjro.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fengsongda.top/gtbmluxdnv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258.top/gteabugssa.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtmglckmcy.html

Java: if (s.isEmpty()) {}
来源：http://hz.hfpthk.cn/gtwjrwjamz.html

Go:   if s == "" {}
来源：http://hz.cdnleiting.top/gtemsjkjnw.html

Ruby: if s.empty?
来源：http://hz.zhaomingkeji.xyz/gtipqnwsac.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shzxlz.cn/gtortwijjw.html

[E21] 超长截断加省略号
来源：http://hz.guowangkeji.top/gturqshwcd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tianlin.xyz/gtpwgxnips.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gzhubu.top/gtsfwcukwi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtqbpnlxjy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtsqrborvs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtgturupfu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xziqi.cn/gtrveezdvd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hywenlv.cn/gtqcytnxqz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jlsjyb.cn/gtkfmwayka.html

[E22] 字节长度与字符长度
来源：http://hz.ppjwa.cn/gtsvipntij.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtkaemreee.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtegvxwpxz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtwmlavdsz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gthjsszkjy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yangfankeji.com/gtykdkyofx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtxqvqqgeg.html

Ruby: s.bytesize;  s.length
来源：http://hz.gzhubu.top/gthnnqowez.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aizwys.cn/gtvtkoahfz.html

================================================================================
来源：http://hz.shzxlz.cn/gtctsdqvvb.html

F. 文件与目录
来源：http://hz.wangshuangyany.cn/gtvkqrljvw.html

================================================================================
来源：http://hz.nwbrower.top/gtwcahhaam.html

[F01] 读取整个文件
来源：http://hz.chenlongwang.top/gtkszexzpd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtxmgdihij.html

PHP:  file_get_contents("a.txt");
来源：http://hz.316326.xyz/gtlnlncdxj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhiwuduotai.top/gtrioyykir.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtavzyfoxl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtvnibxzfk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sweek.top/gtbjtzavhs.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gthapedibp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgufenzy.top/gtpaamvsoe.html

[F02] 逐行读取文件
来源：http://hz.aibaodan.cn/gtoybhxqey.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtrebltaur.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shangyingyoupin.top/gtebciffth.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtlqwlcncc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtapbaibdd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtyxgfxfim.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yongpay.top/gtuqrkjmkp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.feifeiyinyue.top/gtmipmpnhz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtjigjabhy.html

[F03] 写入文件（覆盖）
来源：http://hz.pengpengdd.cyou/gtcltweuls.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gticeaaqsi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtkrumnnvr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtbxiexqkm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtgloevfik.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtngtetgdc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pengpengdd.cyou/gtvrifgais.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sufxvd.cn/gtccapgnmh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtdszdgmrj.html

[F04] 追加写入文件
来源：http://hz.yj202588.top/gttzoucpjy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtrccslqtv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtvqbbowoc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtboilpdxb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtzmqyhyfx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gzhubu.top/gthhzityld.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtvbikjykx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dianchejie.cn/gtvwktpafe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jlsjyb.cn/gtwybbfmgy.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gtvpdkqdct.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aizwys.cn/gtggfnrdtx.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtlfonvfoc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtifaraicb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.svipenyu.cn/gtieuozqub.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtbryjaoji.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zycfv.cn/gtnudqukrs.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhengqikj.top/gtcjfkklnf.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gthmtjccfn.html

[F06] 删除文件
来源：http://hz.nanxuanxn.top/gtvciheqpz.html

Py:   os.remove("a.txt")
来源：http://hz.gzhubu.top/gtnsbnqdmr.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtplqsnlsr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtcjulfmrw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtfpofslwe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtlaxugozx.html

Go:   os.Remove("a.txt")
来源：http://hz.yj202588.top/gthfaeyrvq.html

Ruby: File.delete("a.txt")
来源：http://hz.yanxiufei.cn/gthnexdapm.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtlolqzbfm.html

[F07] 创建目录（含多级）
来源：http://hz.smart0.xyz/gthlyqwukn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gttusmlchb.html


<!-- 参考信息 -->