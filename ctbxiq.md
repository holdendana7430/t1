代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tian-w.cn/gtoujayjry.html

[D20] 统计每个元素出现次数
来源：http://hz.aibaodan.cn/gtfyodjyyp.html

Py:   Counter(arr)
来源：http://hz.fzhhl.top/gtfdlludob.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtjaptccna.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtlwnpysju.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gthovifxvm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.andypj.xyz/gtzuqejfdm.html

Go:   // 手写 map[T]int
来源：http://hz.jqgfzy.top/gttavdnqpk.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtqbyffmwv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtpdcwbgdi.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtsfyczcsp.html

Py:   x in arr
来源：http://hz.shuidangran.top/gteypvtuet.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gtqjscmxga.html

JS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gtfzfbpbww.html

TS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtmkrrbqfi.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtqvkohixw.html

Go:   slices.Contains(arr, x)
来源：http://hz.meibo888.top/gtcnnjhvsz.html

Ruby: arr.include?(x)
来源：http://hz.haohaochexian.top/gtyiftzjqi.html

C#:   list.Contains(x)
来源：http://hz.jinqigufen.top/gtmkeampea.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aizwys.cn/gtgoseuteb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtkvhstysv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daria6918.cn/gtuamlzepz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gzhubu.top/gthrcvdmem.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtawsmnful.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gtmrrlpums.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gtstdbhmnp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dianchejie.cn/gtavqucjxt.html

C#:   new List<int>(list);
来源：http://hz.ybcxt.top/gtdpsdwpjw.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtarnsupyy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yonumen.top/gttpgqidyk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yangfankeji.com/gtxngddoei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtcsxwowin.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtvprtioaq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtxfeuzvpm.html

Go:   // 手写循环
来源：http://hz.sysykeji.top/gtwdsiaooe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.vqdsnc.cn/gtdrdsgwku.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtphpvwory.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtvardbasc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtxnjekhuc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.meibo888.top/gtelgxruzs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenlongwang.top/gtbkiyldsf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.snrcjt.cn/gtpfckvuox.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dashuyun.cn/gtjrfunjnn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gtwfrceduf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shangyingyoupin.top/gtnxavwsam.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hammf.cn/gtgeewlarw.html

[D25] Set 集合去重与交并差
来源：http://hz.hywenlv.cn/gtxymaydsk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hysaishi.cn/gtzzcizwco.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtggzilgko.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gzhubu.top/gtoobuvorb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.havefunace.top/gtlpymgbal.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.birdmap.top/gtlovxxtqm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtlashyakd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtzyfvxwxj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtogvvouvg.html

[D26] 数组转字符串
来源：http://hz.chenlongwang.top/gtnnyaomrx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.316326.xyz/gtmuzqmurv.html

PHP:  implode(", ", $arr);
来源：http://hz.svipenyu.cn/gtxamrsasn.html

JS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtxtvfrgix.html

TS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtwhnbzncg.html

Java: String.join(", ", list)
来源：http://hz.daxiang520.top/gtpmsofydy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gttsardnoe.html

Ruby: arr.join(", ")
来源：http://hz.yuanzhike.top/gtxmjsvnhh.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gtkylqtpwb.html

================================================================================
来源：http://hz.gzhubu.top/gttbbnknvf.html

E. 字符串处理
来源：http://hz.smart0.xyz/gtzeyzaqqv.html

================================================================================
来源：http://hz.yueranfly.top/gtrmaufuqw.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtosvpkccl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gogol.net.cn/gtpsyyljtw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hywenlv.cn/gtjttrspuw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dashuyun.cn/gtwgstmliy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtvvontgmp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.vqdsnc.cn/gtloraxfxa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cashguo.top/gtctrtdjwo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.redwolf501.top/gtgzjtuhnu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.snrcjt.cn/gtcaczfiyc.html

[E02] 重复字符串
来源：http://hz.hfpthk.cn/gtbztmfjxa.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtiikqxqrr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhiwuduotai.top/gtbhisvtwz.html

JS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtdnskkzcs.html

TS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtmmvlbqee.html

Java: "ab".repeat(3)
来源：http://hz.xuanzx.com/gtctfynort.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtmolwojce.html

Ruby: "ab" * 3
来源：http://hz.daria6918.cn/gtowcsjyeb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.redwolf501.top/gtxjiisgww.html

[E03] 截取子串
来源：http://hz.ppjwa.cn/gtaekummao.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenzaomai.com/gtoulhnowi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fzhhl.top/gtotyfboaf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtxoepojko.html

TS:   s.slice(1, 4)
来源：http://hz.gotoacloud.top/gtnfeturzo.html

Java: s.substring(1, 4)
来源：http://hz.nwbrower.top/gtuxvodoog.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtclayeikd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yangfankeji.com/gtwwzcjael.html

C#:   s.Substring(1, 3)
来源：http://hz.jinyuanbaomall.cn/gtfsaojitw.html

[E04] 查找子串位置
来源：http://hz.xuanzx.com/gtcxfootey.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ehwqpu.com/gtbcrtrfqr.html

PHP:  strpos($s, "x");
来源：http://hz.jinghuilouyu.cn/gtwmdduknp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuanzhike.top/gtxepqqgyk.html

TS:   s.indexOf("x")
来源：http://hz.yvedp.cn/gtyrhkcvlh.html

Java: s.indexOf("x")
来源：http://hz.shzxlz.cn/gteptenrua.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gtgvodyavv.html

Ruby: s.index("x")
来源：http://hz.hfpthk.cn/gtjwvchcjk.html

C#:   s.IndexOf("x")
来源：http://hz.hammf.cn/gtccupkbye.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sysykeji.top/gthtpuehjl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cucudq.cn/gtmvoqvzua.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ywan-chungtsiang.top/gtvgcuiofe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gthyrkcbmk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtzwtzzjzy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtehosslnf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xziqi.cn/gtuwoyaktn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pengpengdd.cyou/gthjrmndfk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cashguo.top/gtkvsvvjfo.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gtfogldsqo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtsqwxjoka.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xylfe.cn/gtakvnipmv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gthuywzple.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtxfbwjvyz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtptajapdg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.svipenyu.cn/gtyxfrkoww.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.pengpengdd.cyou/gtilwzlore.html

C#:   s.Replace("a", "b")
来源：http://hz.iojbl.cn/gtsbcigfem.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtndvjwpgk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuanzhike.top/gthaxtqbsk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gtaejvjumo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yvedp.cn/gtoxwnzmfw.html

TS:   s.split(",")
来源：http://hz.cheryme.top/gtedsggwzr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yvedp.cn/gtcwwvmfvn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxinkj.top/gtypgdymel.html

Ruby: s.split(",");  s.split
来源：http://hz.quarkkingdee.top/gtajlbtvqv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinyuanbaomall.cn/gtgrozbgiv.html

[E08] 数组按分隔符合并
来源：http://hz.cucudq.cn/gtgdhfegun.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtbanxprvf.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtbxobmtpu.html

JS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtnsoaeazw.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtjxubkpge.html

Java: String.join(",", items)
来源：http://hz.jqgfzy.top/gtsjauerjo.html

Go:   strings.Join(items, ",")
来源：http://hz.wangdashe.top/gtlyyvcxwy.html

Ruby: items.join(",")
来源：http://hz.xinyue.icu/gtlbmnjpnv.html

C#:   string.Join(",", items)
来源：http://hz.snrcjt.cn/gtkhldkllq.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtgclodkwg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gaohongyu789.top/gttvtoqlyx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ybcxt.top/gteuwfssfs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtuymirekh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.redwolf501.top/gtikxvjsmz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtsszcqgun.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sxryk.cn/gthqhhdfsg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yanxiufei.cn/gttfnomrom.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.feifeiyinyue.top/gtpgkrnwqq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtskqrrmin.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zycfv.cn/gtlorjbifw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.meibo888.top/gtfgdcpcri.html

JS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtswufgekf.html

TS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtyhleyken.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtfskxqlmq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yongpay.top/gtpuokwepa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gttfsnpffn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtkxpuokvn.html

[E11] 反转字符串
来源：http://hz.gotoacloud.top/gtoaztbnnv.html

Py:   s[::-1]
来源：http://hz.mhx1999.top/gtqmslirti.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtpgxmgfoj.html

JS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtxxxloyzj.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtuqnvnixq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xylfe.cn/gtloftqzan.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtgfpqtmtf.html

Ruby: s.reverse
来源：http://hz.zdqjudy.top/gtapczodim.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtprazlozl.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gtpzznkqxs.html

Py:   s.count("a")
来源：http://hz.ivvv.top/gtmphtbhax.html

PHP:  substr_count($s, "a");
来源：http://hz.tanke756.top/gtcsygdynu.html

JS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gthddajqkh.html

TS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtkifoylzg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gogol.net.cn/gtklftqwap.html

Go:   strings.Count(s, "a")
来源：http://hz.xingfuxueyuan.xyz/gtlgmdowup.html

Ruby: s.count("a")
来源：http://hz.daria6918.cn/gtunxjfqvn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtattovgrg.html

[E13] 逐字符遍历
来源：http://hz.jiagoushi.top/gtpilfbrit.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gthnkgqbdp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.meibo888.top/gtxjsrpwki.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtvuwwchfe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtuhjnkemv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.dashuyun.cn/gthyoehehr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtidgwvmiq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gtxxnwccnc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.vqdsnc.cn/gtudphnevf.html

[E14] URL 编码与 Base64
来源：http://hz.quarkkingdee.top/gtojgwnrzw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yongpay.top/gtgwvlebdk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daria6918.cn/gtfxmyzfhc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.9152youxi.cn/gtznycmify.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtyacjdccz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtfnbmjozv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgufenzy.top/gtlnzmkwge.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtzvnenicw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtimwocyxm.html

[E15] HTML 转义 / 反转义
来源：http://hz.birdmap.top/gtmtjqkbeo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hongshengwenyu.top/gtqjctjzer.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gtxoqkdbbk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.wangdashe.top/gtrfiwiimw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtxfncqmeg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.9152youxi.cn/gthcewnffm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yongpay.top/gtlxmywuga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cqqwz.cn/gtueqlasku.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nwbrower.top/gtxybaflfq.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtzycglhnb.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gtiyxouhku.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtxdelqaam.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtqxzvncoq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gttguopzzg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.9152youxi.cn/gtlpbaxbvi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tian-w.cn/gtfeixmosk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gttfolwads.html

C#:   1234567.ToString("N0")
来源：http://hz.iojbl.cn/gtclzhtezd.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtuzvvmtdh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.redwolf501.top/gthfnibysp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenzaomai.com/gtffavyhxj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtbwbqnvxl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtziwzqttd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gtojevuyia.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gtnenyvaym.html

Ruby: s.capitalize
来源：http://hz.gaohongyu789.top/gtkrmpcjpq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gttzdqmofg.html

[E18] 模板占位符替换
来源：http://hz.ydzc1.top/gtggrqzptw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tian-w.cn/gtgaxztcow.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgfzy.top/gtqcvslmfe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtixtkyjnx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtjdgzqnkp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ivvv.top/gtcaugzhmd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangtech.top/gtauljhein.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxinkj.top/gteunscvce.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gaohongyu789.top/gtvigmnqiy.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtfmmmwipr.html

Py:   s.splitlines()
来源：http://hz.hywenlv.cn/gtayqgimqx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhiwuduotai.top/gtpnpykges.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtiinvudnd.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtakprlyzc.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtxmohnuwh.html

Go:   strings.Split(s, "\n")
来源：http://hz.jiagoushi.top/gticsvyoco.html

Ruby: s.lines
来源：http://hz.shangyingyoupin.top/gtnzfaommu.html

C#:   s.Split('\n')
来源：http://hz.c1oappe.top/gtrflafovf.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtdyjarctk.html

Py:   if not s:
来源：http://hz.cqqwz.cn/gtmrumlotv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuanzx.com/gtqzuqtiei.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtxskaaalm.html

TS:   if (s === "") {}
来源：http://hz.wangdashe.top/gtswzkyckp.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtjdzgmpfv.html

Go:   if s == "" {}
来源：http://hz.smart0.xyz/gtelbtzwfh.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtflgwngrb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shzxlz.cn/gthhuoesru.html

[E21] 超长截断加省略号
来源：http://hz.yueranfly.top/gtybwgdkal.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ehwqpu.com/gtiynqnujh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.52xcode.cn/gtimamhpqb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtukotuaop.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtzccrsakl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gteauaxutz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnxiangtu.top/gtqfmluxrq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258.top/gtwuqscvgo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.mhx1999.top/gtmcanctsp.html

[E22] 字节长度与字符长度
来源：http://hz.xingfuxueyuan.xyz/gtpudguico.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangshuangyany.cn/gtaxhwatih.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtisfbodsx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtdpvitqwe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtebxnxslf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtwurqkgxx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gtmflghqrk.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtqzoyxmpb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtlstqmxsv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtystoecqp.html

F. 文件与目录
来源：http://hz.ivvv.top/gtuwfymnaw.html

================================================================================
来源：http://hz.ydzc1.top/gtjxpeflsc.html

[F01] 读取整个文件
来源：http://hz.zhaomingkeji.xyz/gtlkbljuns.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtaddzljbl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuanzhike.top/gtnzwlokzc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yueranfly.top/gtpxxhrbcz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtpknzwcuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtrqkfuruj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.smart0.xyz/gtreikbdrz.html

Ruby: File.read("a.txt")
来源：http://hz.shangyingyoupin.top/gtptixvovj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.daria6918.cn/gtyyzdnuxq.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtnesyjjkj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtcoxfhvgv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gticwpegzt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtgzazoexy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtkuctogvz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtkvmxmwav.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guowangkeji.top/gtkumioxmy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gtzxvedaxf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aibaodan.cn/gtjxlxentk.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtlqjqixrp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtnadnupmm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnqzz.top/gthjqhssac.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtuxrirjij.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtqjzcqqav.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gtgkfpjhif.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zdqjudy.top/gtbhaipwjw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtsyhalivc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gttrfmvsql.html

[F04] 追加写入文件
来源：http://hz.quarkkingdee.top/gtxfyjscfu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gaohongyu789.top/gthktgffbj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtahmiqbjf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtcwqejhip.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtwxyhhiex.html


<!-- 参考信息 -->