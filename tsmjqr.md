代发 wailian999

Ruby: arr.tally
来源：http://hz.svipenyu.cn/gtoocmvxic.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.birdmap.top/gtwbnovmaw.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gthjswxveu.html

Py:   x in arr
来源：http://hz.fzhhl.top/gtorwgmllw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xingfuxueyuan.xyz/gtunsybasp.html

JS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtvqkoglhq.html

TS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtjhbmwrjw.html

Java: list.contains(x)
来源：http://hz.zdqjudy.top/gthvepnvjy.html

Go:   slices.Contains(arr, x)
来源：http://hz.cashguo.top/gtvzglftiu.html

Ruby: arr.include?(x)
来源：http://hz.52xcode.cn/gttcvvqhnv.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtybzrvylm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtgiqqfily.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shangyingyoupin.top/gtzllzjrmv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.smart0.xyz/gtmgarrzkq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhijiandao.cn/gtzguunvko.html

TS:   [...arr];
来源：http://hz.cqqwz.cn/gtwwmkvucb.html

Java: new ArrayList<>(list);
来源：http://hz.yangfankeji.com/gtpouepevo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hysaishi.cn/gtyzjtkjet.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tanke756.top/gtitggtvts.html

C#:   new List<int>(list);
来源：http://hz.vqdsnc.cn/gticnxbhry.html

[D23] reduce 累积计算
来源：http://hz.jinyuanbaomall.cn/gtorobhsdd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.smart0.xyz/gtchaycmnc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuetiantiany.cn/gtyprcbclo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gthallnbom.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtsjsejkbp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtkyvwbtdz.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtcagjesea.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gtxuipwowt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ywan-chungtsiang.top/gtcopuunfj.html

[D24] 字典 / Map 基本操作
来源：http://hz.dashuyun.cn/gtwjumhuos.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gtdocxarfk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.iojbl.cn/gtihtjurob.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.bjfxy.top/gtvectyail.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtpttqlnsz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtriuizoba.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhixingplan.top/gtdpmoauid.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guannengcc.top/gtedebumfs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jlsjyb.cn/gtgbafoiyh.html

[D25] Set 集合去重与交并差
来源：http://hz.iojbl.cn/gtfbotvwhz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gtdlyepdvb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenjidiqi.icu/gtcxcexyxs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtlbztdidk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guowangkeji.top/gtxkwapzfv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tanke756.top/gtdoufgvmg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.9152youxi.cn/gtvvuasasn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gtjfjcbowp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daria6918.cn/gtkwgpinqj.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtqcmbpzva.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtjtieqley.html

PHP:  implode(", ", $arr);
来源：http://hz.chenzaomai.com/gtzckfasgi.html

JS:   arr.join(", ")
来源：http://hz.cashguo.top/gthhsspuqs.html

TS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtznyldxag.html

Java: String.join(", ", list)
来源：http://hz.meibo888.top/gtmkovawho.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtsvcchont.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gtcfuscjcz.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtczqusxho.html

================================================================================
来源：http://hz.gaohongyu789.top/gtdxdcpbkk.html

E. 字符串处理
来源：http://hz.yongpay.top/gtxxfgsssg.html

================================================================================
来源：http://hz.hysaishi.cn/gthwtfcgqe.html

[E01] 拼接字符串
来源：http://hz.chenzaomai.com/gtfnixfouh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.feifeiyinyue.top/gttiyevahh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtmpbmderx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtiixjumqp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtnxzkivcd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xylfe.cn/gtxknuvubu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuanzx.com/gthkljkfoo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.9152youxi.cn/gtvhicimlk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cucudq.cn/gtynfjejxv.html

[E02] 重复字符串
来源：http://hz.yj202588.top/gtlqxreffr.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtkbvznwby.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gtzwvcjhrq.html

JS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtmjavfwsb.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtuatqpdfl.html

Java: "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtzvccmniw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hysaishi.cn/gtoagpxsqa.html

Ruby: "ab" * 3
来源：http://hz.9152youxi.cn/gtkzdvdddr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.pengpengdd.cyou/gtgfjzzulg.html

[E03] 截取子串
来源：http://hz.feifeiyinyue.top/gtzlqrrpmu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhengqikj.top/gtvgzagazg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtyrphfdmx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtdohegcms.html

TS:   s.slice(1, 4)
来源：http://hz.sysykeji.top/gtmfqrlfev.html

Java: s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtnimcdzks.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinqigfzy.top/gttczhvcve.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtskukqyas.html

C#:   s.Substring(1, 3)
来源：http://hz.haohaochexian.top/gtnicyfskg.html

[E04] 查找子串位置
来源：http://hz.tanke756.top/gtguingkbf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtrxiqeudq.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtorqtsswp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.andypj.xyz/gtdvxdauod.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gtziegbqep.html

Java: s.indexOf("x")
来源：http://hz.chenlongwang.top/gtnidnjhqn.html

Go:   strings.Index(s, "x")
来源：http://hz.yvedp.cn/gtcrwyqqoz.html

Ruby: s.index("x")
来源：http://hz.yanxiufei.cn/gtbygmnvra.html

C#:   s.IndexOf("x")
来源：http://hz.sweek.top/gtsxypjool.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258888.top/gtqugtsstx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenjidiqi.icu/gtuimybtlg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhijiandao.cn/gtqtylgxix.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhongyouzk.top/gtahmguinb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.smart0.xyz/gteohvpsek.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtnoovojhg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hysaishi.cn/gtdvzwcgxf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhijiandao.cn/gtydmbwkyk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenjidiqi.icu/gtnxmzvzos.html

[E06] 替换子串
来源：http://hz.zhongyouzk.top/gtmknrwysy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tian-w.cn/gtpwosjjkv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtxltwurtj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gthyrrcyyw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtunmvqzvr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtefjcsyyi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sysykeji.top/gtdrdozbul.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhixingplan.top/gtosrbqyyi.html

C#:   s.Replace("a", "b")
来源：http://hz.shuidangran.top/gtmcqdzuwz.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtoldevkes.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yongpay.top/gtrifviikf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhoulong.xyz/gtoowobwnm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.9152youxi.cn/gtgfkkrtes.html

TS:   s.split(",")
来源：http://hz.yvedp.cn/gtzqtucsti.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtgrzfcptf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yvedp.cn/gtxwrtlhlk.html

Ruby: s.split(",");  s.split
来源：http://hz.shangyingyoupin.top/gtkaazbxcw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtcnlrasuh.html

[E08] 数组按分隔符合并
来源：http://hz.yangfankeji.com/gtvxikyhoy.html

Py:   ",".join(items)
来源：http://hz.316326.xyz/gtolmcttgv.html

PHP:  implode(",", $items);
来源：http://hz.xinyue.icu/gtqduelusz.html

JS:   items.join(",")
来源：http://hz.cashguo.top/gtzcnmouzi.html

TS:   items.join(",")
来源：http://hz.yuanzhike.top/gtcljhomay.html

Java: String.join(",", items)
来源：http://hz.dianchejie.cn/gtawepubhc.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gtoetvvzux.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtjkbksvvv.html

C#:   string.Join(",", items)
来源：http://hz.guannengcc.top/gtfmiexyas.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtuwbdfrbb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zycfv.cn/gtsvdbluyw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.316326.xyz/gtadayqzcg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtaomjauom.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtzddixqne.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtcqcgiyib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtqsgvfvgx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gthqlpmysb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tian-w.cn/gtnubmilta.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtkpnvlfgh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtlwxkdbaz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sufxvd.cn/gtcaefcdpe.html

JS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtmcyjpmze.html

TS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtagkdjvma.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtncpblxaw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtnmvdaxvr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tanke756.top/gtryktbuti.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.meibo888.top/gthmvxgiht.html

[E11] 反转字符串
来源：http://hz.hammf.cn/gtlwrmxzhj.html

Py:   s[::-1]
来源：http://hz.quarkkingdee.top/gtotuoefso.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtsmyylghz.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtliatohap.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtbkvqfxih.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtopcteblm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cqqwz.cn/gtsggegccv.html

Ruby: s.reverse
来源：http://hz.hfpthk.cn/gtddwhmpqy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtbjswnzbc.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtywbltofi.html

Py:   s.count("a")
来源：http://hz.gaohongyu789.top/gtxwwjbqbg.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtjzjmffkc.html

JS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gttbugzaib.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtysoamajv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gtswtedmnl.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtoepfsijm.html

Ruby: s.count("a")
来源：http://hz.nanxinkj.top/gtyrflbflv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daria6918.cn/gtbpyvvbix.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtyawgsvbw.html

Py:   for ch in s: print(ch)
来源：http://hz.zhengqikj.top/gtvtzlnxlr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxuanxn.top/gtpiaajhir.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtcbwwksek.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtmgtvmgpo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hammf.cn/gtnlbtjvpx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangshuangyany.cn/gttpyxulmr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtkndwilej.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtfetvypgr.html

[E14] URL 编码与 Base64
来源：http://hz.yonumen.top/gtlqxwhpho.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtcpvllvxe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangtech.top/gtbihrtzjt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dianchejie.cn/gtijfjqirq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtxvjaezbp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgfzy.top/gtifnhqccz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pengpengdd.cyou/gtsbrtsowd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hammf.cn/gtenzecwfp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gtuwjuvmgp.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtftectzrp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gtnuwjcnqv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gtiaelozgw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtghmgrslf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtautirgtv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtdrwvyrrl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtggxajnkp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtlmxibowz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtzbwdwefc.html

[E16] 数字千分位
来源：http://hz.nwbrower.top/gtcuiqaufi.html

Py:   f"{1234567:,}"
来源：http://hz.zhongyouzk.top/gtbnilowch.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gtagvvbdbi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtxuueioxw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtofljedvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhengqikj.top/gtsfijvnam.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtwinngoew.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gtmbxaixjz.html

C#:   1234567.ToString("N0")
来源：http://hz.daxiang520.top/gtudzmlpeh.html

[E17] 首字母大写
来源：http://hz.hywenlv.cn/gtnphbtcrh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtyoedspax.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shzxlz.cn/gtufbqipya.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtjsexddvy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtbutkhdmz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtiaovehwo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gtthoxaguw.html

Ruby: s.capitalize
来源：http://hz.zdqjudy.top/gtkqpczzql.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhixingplan.top/gtwnryxycv.html

[E18] 模板占位符替换
来源：http://hz.hongshengwenyu.top/gtqipmunqp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.smart0.xyz/gtfmcfoeyo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuanzhike.top/gtvtpyvuno.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtczcickme.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtielbabtv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ybcxt.top/gtdseaxice.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.feifeiyinyue.top/gtowjcpbde.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.quarkkingdee.top/gttyqslgvn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtjhjnbrmw.html

[E19] 多行文本按行拆分
来源：http://hz.sweek.top/gtigtckumw.html

Py:   s.splitlines()
来源：http://hz.smart0.xyz/gtjxgerbbv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtzwdhbezq.html

JS:   s.split(/\r?\n/)
来源：http://hz.wangdashe.top/gtnruqzhcu.html

TS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtldqripmt.html

Java: s.lines().toList()
来源：http://hz.cashguo.top/gtxderfqum.html

Go:   strings.Split(s, "\n")
来源：http://hz.mhx1999.top/gtjttdwiyv.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gtgqkphzzt.html

C#:   s.Split('\n')
来源：http://hz.hysaishi.cn/gtrrknimju.html

[E20] 判断字符串是否为空
来源：http://hz.nanxinkj.top/gtzwhyfslm.html

Py:   if not s:
来源：http://hz.mhx1999.top/gtrbuhaokn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtmqwmvevk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuanzhike.top/gtphepnzql.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtxmfnqciu.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtcpljjsma.html

Go:   if s == "" {}
来源：http://hz.sysykeji.top/gthibyotoc.html

Ruby: if s.empty?
来源：http://hz.shuidangran.top/gtnyakovgg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtduedrfts.html

[E21] 超长截断加省略号
来源：http://hz.cdnleiting.top/gtkldudqqa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gtbyaqnzxb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.birdmap.top/gtkfprpcjw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtczuyzuwi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtytvhqsos.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtznkxszmz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtfousdgdl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenzaomai.com/gtwqqcdgpf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtzyojnodx.html

[E22] 字节长度与字符长度
来源：http://hz.zhaomingkeji.xyz/gtjyjvgbpa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sxryk.cn/gthieijjwg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtjuzrbtni.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtegvgohwj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtncaptjdz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj202588.top/gturzcqvey.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtozwdxatx.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gtckkoonum.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gtgymdwesz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpepkifyy.html

F. 文件与目录
来源：http://hz.svipenyu.cn/gtintowhrn.html

================================================================================
来源：http://hz.chenzaomai.com/gtegoflhxc.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gttezcpltq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dianchejie.cn/gtenluyzzh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtodnvmfii.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gtekyjtasm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258.top/gtyqkbynwo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtrjmskbbd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gtthntvzwm.html

Ruby: File.read("a.txt")
来源：http://hz.cqqwz.cn/gtpqbzmuen.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.9152youxi.cn/gturmykwcw.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gtupyxplrg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shzxlz.cn/gtdrvjltzf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nwbrower.top/gtfwefriim.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtxjozylec.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtcxsmkoia.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gteiwnlarf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtvudqfdrl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhixingplan.top/gtposwevak.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cashguo.top/gtjmemyisr.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258.top/gtsqwzenrv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtpwgcrqiv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtzjnjfoaj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtqegdfwps.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtcqfjuobc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yueranfly.top/gtewenpqgx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dashuyun.cn/gtbwqnonwu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gogol.net.cn/gtumvcjoro.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtykvchkno.html

[F04] 追加写入文件
来源：http://hz.hywenlv.cn/gtfenomktk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.kuanghao11.cn/gtxxliauzi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gzhubu.top/gthtdsnjak.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtpzzwoicq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtngewanqh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gteaowhzgy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.haohaochexian.top/gtmnfhigtx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jiagoushi.top/gtiqccnxxa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jyoumei.cn/gtzfhosjro.html

[F05] 判断文件或目录是否存在
来源：http://hz.yvedp.cn/gthisiubem.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtfpswgqoz.html

PHP:  file_exists("a.txt");
来源：http://hz.pycfn.com/gtnchlqwnd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtbdmkdkjb.html


<!-- 参考信息 -->