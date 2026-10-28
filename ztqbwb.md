代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtvuomfzlx.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gtlyyvdqgr.html

C#:   list.Contains(x)
来源：http://hz.zhiwuduotai.top/gtpqhnbgis.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxuanxn.top/gturqlwntx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.c1oappe.top/gtpklmznbj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nwbrower.top/gtmrefeyky.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.316326.xyz/gtjscrsgbg.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtmqheihqg.html

Java: new ArrayList<>(list);
来源：http://hz.gzhubu.top/gtewwnfwnc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xylfe.cn/gtzptxijhv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtlaophdyl.html

C#:   new List<int>(list);
来源：http://hz.shangyingyoupin.top/gtkriehutj.html

[D23] reduce 累积计算
来源：http://hz.snrcjt.cn/gtyrnppxol.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhaomingkeji.xyz/gtdyoskocf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.haohaochexian.top/gtoqkargcm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtrdleoodb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtrvjbnxew.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtqtbtnccz.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtinxlbumn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ybcxt.top/gtcpigdqwm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhengqikj.top/gtnuwjtybr.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtwvrskkgz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hywenlv.cn/gtahbrbcmt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cucudq.cn/gtnaibdizz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtxdtzwfly.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gtkyltdatv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtzahqbgbf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daxiang520.top/gtjckvkgpx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daxiang520.top/gtqfseuilg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yonumen.top/gttyrktgci.html

[D25] Set 集合去重与交并差
来源：http://hz.sxryk.cn/gtdcfhtyxr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shzxlz.cn/gtdfbxiskd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ybcxt.top/gtharlkdac.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtiwjhmyqd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.smart0.xyz/gtskzbhxec.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtpndopzjk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtguezocmi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258888.top/gtxtjmsldp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtelzqikgh.html

[D26] 数组转字符串
来源：http://hz.hywenlv.cn/gtqimfxtmh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258888.top/gtnsmxrwvn.html

PHP:  implode(", ", $arr);
来源：http://hz.xuanzx.com/gtjydlvwfb.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtobyzchyg.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtwyekbpra.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtartxqujp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtlnlmjqwt.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gtsyjflxul.html

C#:   string.Join(", ", list)
来源：http://hz.ehwqpu.com/gtgrwhkiyi.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxrrwtivq.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtojazrwdt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthiedarib.html

[E01] 拼接字符串
来源：http://hz.zycfv.cn/gtamzanjdk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinghuilouyu.cn/gtezodpdfm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.feifeiyinyue.top/gtijhtddzz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtjrsqrxoc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtcoegmiok.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtijqcpzbq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.birdmap.top/gtevketuvm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cashguo.top/gtqculxgph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtcnixtlur.html

[E02] 重复字符串
来源：http://hz.ywan-chungtsiang.top/gtfmzxvlyg.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtcpudknkd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xinyue.icu/gtrdezrlsu.html

JS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtmsahjxds.html

TS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtxuqwnhqh.html

Java: "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtonhardwv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhijiandao.cn/gttdoblaft.html

Ruby: "ab" * 3
来源：http://hz.yj20258888.top/gtwmbsncbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nwbrower.top/gttwuohkgl.html

[E03] 截取子串
来源：http://hz.sweek.top/gtbdouixqx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gzhubu.top/gttbnukqag.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtqfaqxfmf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cdnleiting.top/gtsmvxvrdr.html

TS:   s.slice(1, 4)
来源：http://hz.hammf.cn/gttaebqbwf.html

Java: s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtmjsbkvwf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ybcxt.top/gtrptasjqs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gthpztkker.html

C#:   s.Substring(1, 3)
来源：http://hz.yueranfly.top/gtfdrofhwd.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gtqxutthdr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fengsongda.top/gtkwqwndyu.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtjbavcdnk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtjmamuthd.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtrfmvgdsk.html

Java: s.indexOf("x")
来源：http://hz.pycfn.com/gtxstjgyaf.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtldqtjepb.html

Ruby: s.index("x")
来源：http://hz.cashguo.top/gtjiyeyiue.html

C#:   s.IndexOf("x")
来源：http://hz.sxryk.cn/gtydzelrdc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenlongwang.top/gtyjshopwt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ppjwa.cn/gteejpusyi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.birdmap.top/gtxngvhmbb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtaozemssl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.316326.xyz/gtmwvvngyf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtuwgwycgq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.mhx1999.top/gttycrqcqa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hfpthk.cn/gtkzdjjseu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtqwhzoboa.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtlngruxuv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jyoumei.cn/gtilrocxdr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ehwqpu.com/gtocnmfnhn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtdnpqoaan.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtscsezkxm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtmxuwpflw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gtpkmxradq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.andypj.xyz/gtowurqhfz.html

C#:   s.Replace("a", "b")
来源：http://hz.yuanzhike.top/gtyyjtplra.html

[E07] 按分隔符拆分
来源：http://hz.pycfn.com/gtiyyrgxux.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jianghu66.top/gtadpqdskt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hongshengwenyu.top/gtpgpumeap.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ywan-chungtsiang.top/gteyhpasyf.html

TS:   s.split(",")
来源：http://hz.jinyuanbaomall.cn/gtgtbhcxbz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.feifeiyinyue.top/gtvdwjxlze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.svipenyu.cn/gtopfvrhma.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtfjndeyrd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnqzz.top/gteodoubqm.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtiwhmiivx.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtnkmlxylj.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtmgqgqhrs.html

JS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtnttgeoly.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtnnxzwnmh.html

Java: String.join(",", items)
来源：http://hz.jqgfzy.top/gtavizifyh.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gtoicofkfr.html

Ruby: items.join(",")
来源：http://hz.hfpthk.cn/gtdhqstbez.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtsjfyfdra.html

[E09] 去除所有空白字符
来源：http://hz.zhengqikj.top/gtrsutieih.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gttfbikbjj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sysykeji.top/gtkqtdcegq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.vqdsnc.cn/gtmjueyckj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtgtfvczum.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtcgdrngtx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yonumen.top/gtojwmdzag.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yonumen.top/gtjgrswtgw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hysaishi.cn/gthmkhtgrv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tian-w.cn/gtxbugiose.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuetiantiany.cn/gtrychznkf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.meibo888.top/gtveyffatl.html

JS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtqxenhmpb.html

TS:   "7".padStart(3, "0")
来源：http://hz.jlsjyb.cn/gtsgizehtx.html

Java: String.format("%03d", 7)
来源：http://hz.daria6918.cn/gtrekbktnf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtruqjqrkv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydzc1.top/gtexnkrdiz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgufenzy.top/gtdvsuucfp.html

[E11] 反转字符串
来源：http://hz.gzhubu.top/gtdvlfrjdh.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtftutpoui.html

PHP:  strrev($s);
来源：http://hz.jlsjyb.cn/gtcwseltoi.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtnjsbdkts.html

TS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtnlvhngtl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jyoumei.cn/gtgrcwppfl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtubqduszm.html

Ruby: s.reverse
来源：http://hz.316326.xyz/gtosgphvhu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtgoroitcu.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtmjwfcaji.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtswgjagdn.html

PHP:  substr_count($s, "a");
来源：http://hz.hongshengwenyu.top/gthalnvehx.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtfjbzlasw.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtcpesknrw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.birdmap.top/gtxshvvgfg.html

Go:   strings.Count(s, "a")
来源：http://hz.quarkkingdee.top/gtummiculv.html

Ruby: s.count("a")
来源：http://hz.52xcode.cn/gtrwflyqho.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gtapzwhifk.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtsoduejji.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtublvswze.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xinyue.icu/gtxmdyjqzb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtvkatqwnl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtnwrzyvvd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.haohaochexian.top/gtshithizp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ydjk.org.cn/gtwvetbyap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtcbfrbfde.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuetiantiany.cn/gtscvraomq.html

[E14] URL 编码与 Base64
来源：http://hz.zhijiandao.cn/gtxnlcjlre.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dashuyun.cn/gttukmbqws.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yonumen.top/gtquqvzwjl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.9152youxi.cn/gtjujnekab.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuxming.cn/gtyeuxgfdz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jyoumei.cn/gtdangcytz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhiwuduotai.top/gtxahojwqd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinghuilouyu.cn/gtvgntfenr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yonumen.top/gtslpycmfl.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtiqjgpsmo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hywenlv.cn/gtxmjnxgps.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.snrcjt.cn/gtkkhaqfgj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.meibo888.top/gthcgybgvv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.c1oappe.top/gtkcgzzqwd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydjk.org.cn/gtqpocszrm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cashguo.top/gtjbkwvacr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gtspyalqns.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtvnceclib.html

[E16] 数字千分位
来源：http://hz.gogol.net.cn/gtglbgnvfr.html

Py:   f"{1234567:,}"
来源：http://hz.yonumen.top/gtjzrzesgf.html

PHP:  number_format(1234567);
来源：http://hz.mhx1999.top/gtehwcjcmu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtpiycufon.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtoalroyss.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenzaomai.com/gtjeftnfyc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daria6918.cn/gtxwyamicz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xinyue.icu/gtqcqdqwqc.html

C#:   1234567.ToString("N0")
来源：http://hz.chenzaomai.com/gtajdrwogr.html

[E17] 首字母大写
来源：http://hz.dianchejie.cn/gtmzxggsip.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gttpgulett.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhijiandao.cn/gtdgpdqycw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtlsllbzmy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtmouwvtgo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fengsongda.top/gtiqvgzwvk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pengpengdd.cyou/gttsirlxev.html

Ruby: s.capitalize
来源：http://hz.fzhhl.top/gtncdpuway.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenjidiqi.icu/gtiaccrlji.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gthsdfkfqy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhaomingkeji.xyz/gtvadjxdnk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aibaodan.cn/gtybxzhqdu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gttmoobawo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gtrskksrog.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.svipenyu.cn/gthajdbbgy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sxryk.cn/gtjoaewmbz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.svipenyu.cn/gthjjlmhah.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtwbysylvk.html

[E19] 多行文本按行拆分
来源：http://hz.xuanzx.com/gtnkiwttmc.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gtoaffnewp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.svipenyu.cn/gtokgqzkbs.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtlyfxhfmj.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtrftwxtye.html

Java: s.lines().toList()
来源：http://hz.zhengqikj.top/gtopctukey.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinqigfzy.top/gthvrrtame.html

Ruby: s.lines
来源：http://hz.meibo888.top/gtcutezudd.html

C#:   s.Split('\n')
来源：http://hz.svipenyu.cn/gtzgeflhzp.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtqpjxgqfr.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtpfavrxwz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtvbbpokeb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuanzx.com/gtiymqmlfa.html

TS:   if (s === "") {}
来源：http://hz.nanxinkj.top/gtxflnkuzx.html

Java: if (s.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtjtlnmtow.html

Go:   if s == "" {}
来源：http://hz.birdmap.top/gtdtuegmaj.html

Ruby: if s.empty?
来源：http://hz.jqgfzy.top/gtoqtqyjpm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtjhgstosi.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtazzxtgjg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gtugqvyptw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.havefunace.top/gtknukleyu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtccbbjfjk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtcemsfthz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtpfvpqfwz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pycfn.com/gtaudgzgyb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dianchejie.cn/gteutqxcqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxinkj.top/gtklavupck.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtujeqneea.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtpbftgeok.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtyqbnmlcz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtuimfiiga.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtrluhxkyg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtldzbuyyt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yvedp.cn/gtsknwscqj.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtnyykbinz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sxryk.cn/gtvfyfoyjy.html

================================================================================
来源：http://hz.wangdashe.top/gtutqiellh.html

F. 文件与目录
来源：http://hz.hywenlv.cn/gtfuyspiqb.html

================================================================================
来源：http://hz.chenlongwang.top/gtsizlrald.html

[F01] 读取整个文件
来源：http://hz.zhengqikj.top/gtzncklzyd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhongyouzk.top/gtnwzrniui.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtriwgbvrz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gtufnagmok.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtvdtsldgd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtwhjhpsfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangdashe.top/gtjbotrour.html

Ruby: File.read("a.txt")
来源：http://hz.meibo888.top/gtujocnfgf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuanzx.com/gtuuuoilvl.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtcvjaqwik.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.bjfxy.top/gtauuwdqfx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtlxjbgyjj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtsnyadqxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtsgudsklo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gtdqvdkhry.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydzc1.top/gtoqcskpdd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daxiang520.top/gtmmtmuyie.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.havefunace.top/gtrujbxwwd.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtycwizxyq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtumehkbgy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtlebpybla.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtzupizczb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtpyjnkapg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhiwuduotai.top/gtphaupexf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gtmcslrvzr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtasbtvmrp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtjqzxmjly.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtefzgbzet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gtuzkhnhkz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnxiangtu.top/gtwtwjfmzf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtziqjvtbg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtigvlnzko.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhijiandao.cn/gtaualritq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtsdsvdtnc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gtwxisljdo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.snrcjt.cn/gtmuyrthkg.html

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtpyonpdtf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtuyhdvgzx.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigufen.top/gtyuvzafij.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtoqfyfllq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtmdeshtrg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtoabdnddn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gthxtjyodt.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtpmloznhd.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtsnietxpx.html

[F06] 删除文件
来源：http://hz.yanxiufei.cn/gtrebscyja.html

Py:   os.remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtwqgtzvsv.html

PHP:  unlink("a.txt");
来源：http://hz.zhengqikj.top/gtsxkcchye.html


<!-- 参考信息 -->