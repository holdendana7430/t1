代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtfotfcbfe.html

JS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtouwfohnl.html

TS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtrbpquljy.html

Java: list.contains(x)
来源：http://hz.9152youxi.cn/gtqxjcrelk.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenlongwang.top/gtaotivdvn.html

Ruby: arr.include?(x)
来源：http://hz.jinqigufen.top/gtxertbbeh.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gtdglmustn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtehhlaoxe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhixingplan.top/gtztcagtmq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangshuangyany.cn/gtnxvnkamx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtifljmtty.html

TS:   [...arr];
来源：http://hz.haohaochexian.top/gtoyqeykwn.html

Java: new ArrayList<>(list);
来源：http://hz.ivvv.top/gtsfhdpldy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gtosgpfmlm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenzaomai.com/gtggwzaprw.html

C#:   new List<int>(list);
来源：http://hz.shangyingyoupin.top/gtysdaqbnb.html

[D23] reduce 累积计算
来源：http://hz.jinghuilouyu.cn/gtkmmmqnwu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gttxjpfzsz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydjk.org.cn/gtwmymiuyh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtntrjybjk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtosqnqnrl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cqqwz.cn/gtrdamfpbu.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gttwnascyd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hywenlv.cn/gtwhtobqov.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shangyingyoupin.top/gtoqbtyqhp.html

[D24] 字典 / Map 基本操作
来源：http://hz.daxiang520.top/gtcwrcroiy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigfzy.top/gtgscfqcrg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hysaishi.cn/gtozoftbxe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.52xcode.cn/gtzbjzkyak.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gtzderbqfy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shuidangran.top/gtpytcqdui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.andypj.xyz/gtbkfrfegr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtsykpyyup.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gtdtbiglpe.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtliwoscwq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtmlrhdauw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnxiangtu.top/gtumlqaifg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenzaomai.com/gtonwwhhgo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xingfuxueyuan.xyz/gtwnyzsnxo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yanxiufei.cn/gtgpusrfqo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shuidangran.top/gtltmdmurj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shuidangran.top/gtrgsqgnde.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jyoumei.cn/gthsmeosrj.html

[D26] 数组转字符串
来源：http://hz.xuanzx.com/gtcuglpiou.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gtocwlhxdi.html

PHP:  implode(", ", $arr);
来源：http://hz.zhijiandao.cn/gtcthyinwr.html

JS:   arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtbqitolkc.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtizeafsqd.html

Java: String.join(", ", list)
来源：http://hz.birdmap.top/gtllttvafo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtjbsqdtqr.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtvalwrnxy.html

C#:   string.Join(", ", list)
来源：http://hz.yangfankeji.com/gtqkupxnaz.html

================================================================================
来源：http://hz.cucudq.cn/gtgfujuyrd.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gttuciupei.html

================================================================================
来源：http://hz.ppjwa.cn/gtbbabsxen.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gtpbfvdnkm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tianlin.xyz/gtwyrdghfi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhoulong.xyz/gterslvptk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gtabcqzxwa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtezheomsj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.meibo888.top/gtbsafkfla.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gtnyywauul.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shuidangran.top/gtvxltutok.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gtqhwmnyra.html

[E02] 重复字符串
来源：http://hz.ywan-chungtsiang.top/gtosciaehc.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtaznysltd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gtrfnfnqeh.html

JS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtdrpcxmhf.html

TS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtzxuppwmv.html

Java: "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtcddyqqoi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenzaomai.com/gttsdnyfrs.html

Ruby: "ab" * 3
来源：http://hz.ybcxt.top/gtjfrsgmhi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xylfe.cn/gtsodffwnu.html

[E03] 截取子串
来源：http://hz.jinqigufen.top/gtrdewnrzj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fzhhl.top/gtvayjtlmf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtqvdhzshv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtczpfzlxr.html

TS:   s.slice(1, 4)
来源：http://hz.vqdsnc.cn/gtiazsexvj.html

Java: s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtepknluya.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xziqi.cn/gttegxbeuu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.52xcode.cn/gthcoefvqk.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtwyyjawtn.html

[E04] 查找子串位置
来源：http://hz.jinghuilouyu.cn/gtrsaeshmf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cucudq.cn/gtdrqgnueb.html

PHP:  strpos($s, "x");
来源：http://hz.sweek.top/gtsdtsykhw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tian-w.cn/gtmbpghkwl.html

TS:   s.indexOf("x")
来源：http://hz.meibo888.top/gtcqiixgmx.html

Java: s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtmlkofuja.html

Go:   strings.Index(s, "x")
来源：http://hz.zycfv.cn/gtlbzdfhfg.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gttbnxgoim.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtjqbtijgp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.andypj.xyz/gtkgbxzvml.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.bjfxy.top/gtfhuuohzh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pycfn.com/gtdmvgpnfy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtoatxvryr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtdxlyzdmd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtsolathph.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jyoumei.cn/gtbbeewjll.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtklvvqcuj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhiwuduotai.top/gtpdkrvbgv.html

[E06] 替换子串
来源：http://hz.havefunace.top/gtlgrptfcc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.daria6918.cn/gtscabljtt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtgmpuhbve.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtqtoshhlo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtyxlgwgpl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtjahxilwe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gotoacloud.top/gtzgbakjrw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gzhubu.top/gtfolkdyio.html

C#:   s.Replace("a", "b")
来源：http://hz.redwolf501.top/gtjxhxvbfj.html

[E07] 按分隔符拆分
来源：http://hz.jiagoushi.top/gtagcfbjce.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gtuwnkcbsc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhixingplan.top/gtdgqkqdka.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtrjbskvad.html

TS:   s.split(",")
来源：http://hz.jinqigfzy.top/gtvsfjbgce.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtesuyiqbu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yueranfly.top/gtnyhbteno.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gtzhtgxubq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhiwuduotai.top/gtjytjaxyq.html

[E08] 数组按分隔符合并
来源：http://hz.nanxinkj.top/gtpckvcqzq.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtoixxrefi.html

PHP:  implode(",", $items);
来源：http://hz.chenlongwang.top/gtuuigdijz.html

JS:   items.join(",")
来源：http://hz.sweek.top/gtdeqkpigb.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtakgookfb.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtcpeocaof.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxuanxn.top/gtasbfdane.html

Ruby: items.join(",")
来源：http://hz.tianlin.xyz/gthbjnhqrm.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtyrmdfspt.html

[E09] 去除所有空白字符
来源：http://hz.gotoacloud.top/gtslhdmsoz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gthvowvqqb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxuanxn.top/gtkogresxu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gogol.net.cn/gtzlbbdhbi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gtfphiyqcn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guannengcc.top/gtnntqhrhm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtywgmewhi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yanxiufei.cn/gtsbuymuso.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fzhhl.top/gthcvonzkn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtedmtppoj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gtdavoeukq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtqgeuzmwm.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtwxjdfegj.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtjlepehlk.html

Java: String.format("%03d", 7)
来源：http://hz.zycfv.cn/gtywmpxrdx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtzatwydbc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gthggxrnth.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ybcxt.top/gtkqydnfpe.html

[E11] 反转字符串
来源：http://hz.shuidangran.top/gtffpozeaa.html

Py:   s[::-1]
来源：http://hz.birdmap.top/gtvjkzqykb.html

PHP:  strrev($s);
来源：http://hz.yongpay.top/gtookdgbsp.html

JS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtazoacrcy.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtcfowqccp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yongpay.top/gtsdhvvmal.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shzxlz.cn/gtvawijbyu.html

Ruby: s.reverse
来源：http://hz.nanxinkj.top/gtwkbtkorp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtonphoacb.html

[E12] 统计某字符出现次数
来源：http://hz.birdmap.top/gthdgbkydf.html

Py:   s.count("a")
来源：http://hz.sufxvd.cn/gtlfjrfpkw.html

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gtkafeoagq.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtslfgumih.html

TS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtwsieycsg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cqqwz.cn/gtobkkhyef.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtrxsjbtys.html

Ruby: s.count("a")
来源：http://hz.jinqigfzy.top/gtdaylondv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtgavnthqw.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gthdykphjb.html

Py:   for ch in s: print(ch)
来源：http://hz.c1oappe.top/gtpxhoxafw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuxming.cn/gtozagffrh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtprzmmteb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtetrmbprh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuxming.cn/gtaijuokmr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hongshengwenyu.top/gtgiipajbs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtoykacqud.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.snrcjt.cn/gtuslirjff.html

[E14] URL 编码与 Base64
来源：http://hz.shzxlz.cn/gthiyzdepa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.daxiang520.top/gteuvtnegw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gtjrtjlyba.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aibaodan.cn/gtndecwhkd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gaohongyu789.top/gtfdapbwjv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fzhhl.top/gttkmzlnzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jlsjyb.cn/gtorrxncjd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aibaodan.cn/gtfqzuampb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtnsfamsez.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtrrccmojc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gthoqtnmfm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sxryk.cn/gtusaivdac.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuetiantiany.cn/gthcrwnlkk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhiwuduotai.top/gtelwwajlc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sweek.top/gtkzlgjrel.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ehwqpu.com/gttqwwfpga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gaohongyu789.top/gtaaxrboim.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dashuyun.cn/gtljyyouog.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtavsnunhd.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtakbnhwal.html

PHP:  number_format(1234567);
来源：http://hz.c1oappe.top/gtlpibsbvv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtcgznrqkd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtfmhximjh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daxiang520.top/gtgenjgzan.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ppjwa.cn/gthajjvdvg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtydfgtbun.html

C#:   1234567.ToString("N0")
来源：http://hz.zhongyouzk.top/gtvbldgxyn.html

[E17] 首字母大写
来源：http://hz.jiagoushi.top/gtbodgjilg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtmjkckvmg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hongshengwenyu.top/gtvmdktnag.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtfbdkdiji.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtojthpzvs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.quarkkingdee.top/gtpsbxhzyp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtshgleiwo.html

Ruby: s.capitalize
来源：http://hz.jianghu66.top/gtdrzxldig.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hnxiangtu.top/gtkcpfbxcc.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtbqbuksby.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gtxyuaroam.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhongyouzk.top/gtmswaseka.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtgaejrjpr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtbrkylhsh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtrdnowftr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yvedp.cn/gtpoiczrrk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sxryk.cn/gttiopsgvo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gotoacloud.top/gtljtqynxh.html

[E19] 多行文本按行拆分
来源：http://hz.zhongyouzk.top/gtsdexwyan.html

Py:   s.splitlines()
来源：http://hz.wangshuangyany.cn/gtmgyretkg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258.top/gtsxhqlxbf.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtwloudilc.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangdashe.top/gtrfjheapr.html

Java: s.lines().toList()
来源：http://hz.jianghu66.top/gtcnojrnke.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinyuanbaomall.cn/gtqzhsxlus.html

Ruby: s.lines
来源：http://hz.gzhubu.top/gtygjlrsby.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtvkzbsuum.html

[E20] 判断字符串是否为空
来源：http://hz.ywan-chungtsiang.top/gtwfhihaao.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtgvxufbvd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.redwolf501.top/gtpwduacbw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtdshvwgxr.html

TS:   if (s === "") {}
来源：http://hz.ppjwa.cn/gthrgvpamo.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gthlrsvubv.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtqtqafzjp.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtxakmmzqa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jyoumei.cn/gtefihmbzc.html

[E21] 超长截断加省略号
来源：http://hz.nwbrower.top/gtyyohgmtj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gtwdcnucjc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gthhpmtsbn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtlbhyvedb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtbslbmulg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtndvhvawv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtaemdwlxl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.haohaochexian.top/gtrzriglga.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtyrcbambz.html

[E22] 字节长度与字符长度
来源：http://hz.cqqwz.cn/gtyniirhom.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhaomingkeji.xyz/gtcoxzuvvc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtztrzifzx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtdcdnbght.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtfslayhpc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shangyingyoupin.top/gtjszjdzto.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fzhhl.top/gtlvpzuasq.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtdooozrli.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ppjwa.cn/gtroghtoyu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxtrjyxyr.html

F. 文件与目录
来源：http://hz.zycfv.cn/gthwutaaty.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxoxwpdez.html

[F01] 读取整个文件
来源：http://hz.svipenyu.cn/gtpuaamesz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.feifeiyinyue.top/gtdvjkhvzn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sufxvd.cn/gtwxheiywj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.havefunace.top/gtlnyyccph.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gtmppfoumz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtizgiusdj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtycshgxml.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtswgsziur.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangtech.top/gtbfaxuzgp.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtecuvzytm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.smart0.xyz/gtxcoazmbj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtpeztkrxj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtoqnjseol.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtrwugotyf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtldkxtqoh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangtech.top/gtkseitkzj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtybipdjma.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtvikwnwik.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gtzmyaklof.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gthyndiqos.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtoximgaye.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtneposbbh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtfwmryqvr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtcvjqqqox.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtrshqrkjx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gtpialfhvi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258888.top/gtpgyfluyt.html

[F04] 追加写入文件
来源：http://hz.316326.xyz/gttslwkjpv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gthpgccawk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ehwqpu.com/gtapmqeosn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtafitdugp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhengqikj.top/gtfafbjprg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yvedp.cn/gtghqqvzkk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gttocwlphj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yonumen.top/gtszkehucf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtthqtngts.html

[F05] 判断文件或目录是否存在
来源：http://hz.cdnleiting.top/gtfljjtyyr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cqqwz.cn/gtlmigvret.html

PHP:  file_exists("a.txt");
来源：http://hz.birdmap.top/gtvlqqmjty.html

JS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gthkagcxqk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtywhumnkq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtxhumtaya.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guannengcc.top/gtcmxtcdzy.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangshuangyany.cn/gtnufnvbmy.html


<!-- 参考信息 -->