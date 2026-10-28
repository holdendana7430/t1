代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.zycfv.cn/gtuygsamtp.html

Ruby: arr.include?(x)
来源：http://hz.yanxiufei.cn/gtzrqcqilk.html

C#:   list.Contains(x)
来源：http://hz.haohaochexian.top/gtqzfgyaks.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nwbrower.top/gtxcqjgaed.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtatncnngz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gtwhxbmxtx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xingfuxueyuan.xyz/gtghiizkdu.html

TS:   [...arr];
来源：http://hz.meibo888.top/gtgysmuzyz.html

Java: new ArrayList<>(list);
来源：http://hz.shzxlz.cn/gtclsvkndy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtpjtiqchg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gteuwjxhwn.html

C#:   new List<int>(list);
来源：http://hz.0kj1m.cn/gtgqwpdfdd.html

[D23] reduce 累积计算
来源：http://hz.guowangkeji.top/gtpfxtjqdd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shangyingyoupin.top/gtbhesobxs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhiwuduotai.top/gtfvztxqbb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtrhwbknrf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtdmtjeucm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gtitujpgyt.html

Go:   // 手写循环
来源：http://hz.redwolf501.top/gtxezrnzub.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yuanzhike.top/gtfhssxdqv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tanke756.top/gtomxaehjz.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtxbvlphpe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tian-w.cn/gtzyixeqfd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258888.top/gtwedpghar.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.kuanghao11.cn/gtbzikkihv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ivvv.top/gtvvdzzawb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangdashe.top/gttdtzesrp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtpxrjcbvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gtaagoazfc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gtkghqnrsv.html

[D25] Set 集合去重与交并差
来源：http://hz.hongshengwenyu.top/gtesgwwltw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gtahwaeqee.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangshuangyany.cn/gtqzxwsbub.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuanzx.com/gtelhkundz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sxryk.cn/gtzxakcvjh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dashuyun.cn/gttdeloybh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtmxwkkymg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gthgzpbmfy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yvedp.cn/gtshuecnsx.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtzogmvquu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gteftjgrym.html

PHP:  implode(", ", $arr);
来源：http://hz.cqqwz.cn/gteaxwbnhb.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtldndekts.html

TS:   arr.join(", ")
来源：http://hz.shzxlz.cn/gtxtvnmmwi.html

Java: String.join(", ", list)
来源：http://hz.dianchejie.cn/gtgozyadtv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.kuanghao11.cn/gtvnidfnhl.html

Ruby: arr.join(", ")
来源：http://hz.chenzaomai.com/gtjypuuwhi.html

C#:   string.Join(", ", list)
来源：http://hz.andypj.xyz/gtxpbdnpfd.html

================================================================================
来源：http://hz.ehwqpu.com/gtaywtanbc.html

E. 字符串处理
来源：http://hz.xingfuxueyuan.xyz/gtyrfoagok.html

================================================================================
来源：http://hz.guowangkeji.top/gtywtbtugz.html

[E01] 拼接字符串
来源：http://hz.cqqwz.cn/gtvifshdvx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuetiantiany.cn/gtbszbtfog.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zdqjudy.top/gtedrdilqm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gtvbgchupo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtvcxyfvmx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yanxiufei.cn/gtodyscgro.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gtmczyhcmi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhiwuduotai.top/gtqrgnbtyc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.9152youxi.cn/gtvhlajtnf.html

[E02] 重复字符串
来源：http://hz.yj20258.top/gtfsbitchf.html

Py:   "ab" * 3
来源：http://hz.jyoumei.cn/gtdekieotm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xinyue.icu/gtwnhszcsu.html

JS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtjtdhofxb.html

TS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtrcewvvaf.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtplqmcawg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sweek.top/gtpxnvwzrt.html

Ruby: "ab" * 3
来源：http://hz.sysykeji.top/gtlhzgwipv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.quarkkingdee.top/gtpyvimqom.html

[E03] 截取子串
来源：http://hz.sysykeji.top/gtvrbnybmy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gticxytjys.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hammf.cn/gtkamspzfr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tanke756.top/gtrpsmwpdx.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gtxhdxxivm.html

Java: s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtdttaolzi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gthlzhbacl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuanzx.com/gtveuhvaiy.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtdzxzzkzg.html

[E04] 查找子串位置
来源：http://hz.shzxlz.cn/gtezynqrum.html

Py:   s.find("x");  s.index("x")
来源：http://hz.316326.xyz/gtsbjxltju.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gturubvwgj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnqzz.top/gtfblppvis.html

TS:   s.indexOf("x")
来源：http://hz.cashguo.top/gtfjlwwmms.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gtersbndwd.html

Go:   strings.Index(s, "x")
来源：http://hz.mhx1999.top/gtscjzajgo.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtscpxlake.html

C#:   s.IndexOf("x")
来源：http://hz.smart0.xyz/gtzqzutiub.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhiwuduotai.top/gtvdodcqfg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aibaodan.cn/gtrbzhizgd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.0kj1m.cn/gtnqajmfjn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtebzdkhsx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pycfn.com/gtioggfyqr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtmnsmuwwr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gttxyxdijw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigufen.top/gthmmfyprq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.feifeiyinyue.top/gtbegecrud.html

[E06] 替换子串
来源：http://hz.hongshengwenyu.top/gtyioplmyz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yongpay.top/gtvjxvnecs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhaomingkeji.xyz/gtjjfucgjg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gthfabrnll.html

TS:   s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtttctdscr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtmokigwgg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtwqunqlos.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtitcovadm.html

C#:   s.Replace("a", "b")
来源：http://hz.tanke756.top/gtprogccip.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtbesvjruf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigfzy.top/gtaejgltxw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gttgejmgyz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.c1oappe.top/gttappgpui.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtbzjawrpu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gtuwxlvfnr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxuanxn.top/gtegjylaee.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtrcsctqzh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtsdxgnekc.html

[E08] 数组按分隔符合并
来源：http://hz.fengsongda.top/gtgodrrjvl.html

Py:   ",".join(items)
来源：http://hz.chenlongwang.top/gtboylfivf.html

PHP:  implode(",", $items);
来源：http://hz.chenzaomai.com/gtbsbaqfir.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtyunrkzze.html

TS:   items.join(",")
来源：http://hz.hnqzz.top/gtkyjgchcn.html

Java: String.join(",", items)
来源：http://hz.jyoumei.cn/gthepadxhf.html

Go:   strings.Join(items, ",")
来源：http://hz.jianghu66.top/gtmnraelpc.html

Ruby: items.join(",")
来源：http://hz.xuanzx.com/gtngoiyktf.html

C#:   string.Join(",", items)
来源：http://hz.c1oappe.top/gtdjpyxfer.html

[E09] 去除所有空白字符
来源：http://hz.gogol.net.cn/gtpxtplcvw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhiwuduotai.top/gtjvvogdal.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hongshengwenyu.top/gtwhjzixjg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtlvgpmrtt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtpiighqxa.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtywmquhhd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xziqi.cn/gtaulbxpwa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gtemfnltvs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtimqnyhsy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtcxojqeez.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhijiandao.cn/gtzmqnnxeg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.haohaochexian.top/gtdkefocyl.html

JS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtljqdelno.html

TS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtspobxfna.html

Java: String.format("%03d", 7)
来源：http://hz.yueranfly.top/gtmbnfngbn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gthnnxzqdm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtqgfdhieq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gttjxvodgo.html

[E11] 反转字符串
来源：http://hz.sweek.top/gtfktefzlb.html

Py:   s[::-1]
来源：http://hz.shangyingyoupin.top/gtdntqsulc.html

PHP:  strrev($s);
来源：http://hz.guannengcc.top/gtyksawtoe.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtjfawjgav.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtvdxgmfls.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cheryme.top/gtmdyddnjh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtupbyqzpb.html

Ruby: s.reverse
来源：http://hz.iojbl.cn/gtkgdpibxr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtrkvnbblz.html

[E12] 统计某字符出现次数
来源：http://hz.hysaishi.cn/gtytrrjvjg.html

Py:   s.count("a")
来源：http://hz.ybcxt.top/gtzmnwfkvs.html

PHP:  substr_count($s, "a");
来源：http://hz.cdnleiting.top/gtxjcayhqq.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtascjpijx.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangkeji.top/gteyjvmamv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gtvpdvzhnc.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtnhrrmftx.html

Ruby: s.count("a")
来源：http://hz.guannengcc.top/gtpxmmkigg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxuanxn.top/gterewecnh.html

[E13] 逐字符遍历
来源：http://hz.chenlongwang.top/gtkbpojgdp.html

Py:   for ch in s: print(ch)
来源：http://hz.52xcode.cn/gtisdyapcm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xuanzx.com/gtqfxaaxzw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtwhiamkpa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtevklepze.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtzppyysob.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zdqjudy.top/gtettpmbfj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ybcxt.top/gtywazgxgx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hammf.cn/gtwxlkyumy.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gtxkcopszc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258.top/gtbsbzyicy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigfzy.top/gtwzvdexkp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hywenlv.cn/gtxxwcszno.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtwsnghkoe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.vqdsnc.cn/gthddsbdfk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dashuyun.cn/gtrwcosoqt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenlongwang.top/gtqkmceigt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.meibo888.top/gtinfcnrrg.html

[E15] HTML 转义 / 反转义
来源：http://hz.cqqwz.cn/gttckzmdxe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.52xcode.cn/gttqpmigpr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxuanxn.top/gtroppnsty.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gtedyyfkqc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shangyingyoupin.top/gtantirahk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tanke756.top/gtfiuqnubg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jiagoushi.top/gtozazqqjy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtmiehkbso.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gthlewvwng.html

[E16] 数字千分位
来源：http://hz.yj20258888.top/gtcygekhkk.html

Py:   f"{1234567:,}"
来源：http://hz.ywan-chungtsiang.top/gteimecuhw.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtjtyrcegn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtcjafxlbk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtvozjwwha.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hammf.cn/gthchplglu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sysykeji.top/gtlcmwfktt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gtldyiehmc.html

C#:   1234567.ToString("N0")
来源：http://hz.mhx1999.top/gtutcznxdz.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtkohvqflm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtsysmmxau.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtizcfmkvf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gttajebfwq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtpurghwaq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xinyue.icu/gtkldlundf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuetiantiany.cn/gtpwhexplj.html

Ruby: s.capitalize
来源：http://hz.yongpay.top/gtqrazkasv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtmoykaodf.html

[E18] 模板占位符替换
来源：http://hz.316326.xyz/gtijfctumk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258.top/gtebkbulmt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtmaizapwv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gthfliffot.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gthuszdjef.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gteblwmwfu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gtlajtftpa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuanzx.com/gtpfdncfht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtxgbxfqem.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258.top/gtsbimuqpq.html

Py:   s.splitlines()
来源：http://hz.yonumen.top/gtogszychv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gthlrhmnfu.html

JS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtkwefbhcd.html

TS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtlounqwot.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtbvwruwqt.html

Go:   strings.Split(s, "\n")
来源：http://hz.ehwqpu.com/gtjrntxhbp.html

Ruby: s.lines
来源：http://hz.ywan-chungtsiang.top/gtkgluhsje.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtvollxhit.html

[E20] 判断字符串是否为空
来源：http://hz.yuanzhike.top/gtpvggmzzk.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtuafhgbnk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtzesgzbic.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtcpbtkaec.html

TS:   if (s === "") {}
来源：http://hz.iojbl.cn/gtrutahvhu.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtgjqscwvz.html

Go:   if s == "" {}
来源：http://hz.pycfn.com/gtqjltyhls.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtbiodzgyq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zdqjudy.top/gtvwekwnnh.html

[E21] 超长截断加省略号
来源：http://hz.0kj1m.cn/gtrbrbveqa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.meibo888.top/gtvsfmrfaf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gtrpmmbkyc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtgnqfgryi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtjzhxsuct.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtoyzizkxn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xingfuxueyuan.xyz/gtlnyjvczi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtwvgitqlv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtnzjcqkfz.html

[E22] 字节长度与字符长度
来源：http://hz.gzhubu.top/gtykvxzjrq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtqiftzeby.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.smart0.xyz/gttdnwrmsh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gtktmkclgo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cucudq.cn/gtvpazrggm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yuxming.cn/gtbtktaavq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtxfpfayjm.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhiwuduotai.top/gtpjyaxvlk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtghgmbxod.html

================================================================================
来源：http://hz.jinqigufen.top/gtvnrcnubq.html

F. 文件与目录
来源：http://hz.birdmap.top/gtpiuqjrsh.html

================================================================================
来源：http://hz.jinqigufen.top/gtlrmxvkgw.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gtqvozhvzr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnqzz.top/gtpoplrwgt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtgtstfcsg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hfpthk.cn/gtcozfvweu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhijiandao.cn/gtjyinbqec.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtbrfwlgat.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtvvoselop.html

Ruby: File.read("a.txt")
来源：http://hz.mhx1999.top/gtyclanzzi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhijiandao.cn/gtwcvscicq.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtntevitty.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtdzurmxja.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuetiantiany.cn/gtrmdcwcqs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtvegpyitk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtsrsibxnh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtgpeijfdk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xingfuxueyuan.xyz/gtqfqunxzk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gthxbkpkod.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtrapfrahi.html

[F03] 写入文件（覆盖）
来源：http://hz.svipenyu.cn/gtguaxwfac.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.quarkkingdee.top/gtobcriwzo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtfheokdrv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtuiktblqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtismtesnq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cucudq.cn/gtapjctfhf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fzhhl.top/gtkcgadgqn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gtyvlbprxw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtozlqpnkq.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangkeji.top/gttbvhdjxf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258.top/gtylnnswhh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guannengcc.top/gthxeedhmi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtqrerzhle.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtpxlmidpy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cdnleiting.top/gtmmoidqed.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangtech.top/gtvggamxtg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtngmuflne.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gtaqvqmlqh.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtgarnippg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtlfkashmh.html

PHP:  file_exists("a.txt");
来源：http://hz.cheryme.top/gtomtyatec.html

JS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtdnnxcqog.html

TS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtfnqoafpg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtbwqxwfaw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangdashe.top/gtxyxceyoa.html

Ruby: File.exist?("a.txt")
来源：http://hz.yangfankeji.com/gtrnnmkgzm.html

C#:   File.Exists("a.txt")
来源：http://hz.xziqi.cn/gtywxwysbo.html

[F06] 删除文件
来源：http://hz.nanxuanxn.top/gtiwqpyxpd.html

Py:   os.remove("a.txt")
来源：http://hz.jqgufenzy.top/gtxlvspqed.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtpyuahcdg.html


<!-- 参考信息 -->