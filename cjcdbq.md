代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aibaodan.cn/gtvoysjnkz.html

[D20] 统计每个元素出现次数
来源：http://hz.ydzc1.top/gtxdxvedkp.html

Py:   Counter(arr)
来源：http://hz.shangyingyoupin.top/gtfxkwuurr.html

PHP:  array_count_values($arr);
来源：http://hz.ivvv.top/gtvuubvypi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cheryme.top/gtiqhjkwqf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtyemxaqkr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ywan-chungtsiang.top/gtihishtfz.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtpqvipfud.html

Ruby: arr.tally
来源：http://hz.haohaochexian.top/gtigkfvpbm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinghuilouyu.cn/gtqfjldthh.html

[D21] 判断是否包含某元素
来源：http://hz.jianghu66.top/gtfjagnohb.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtrkxxqchw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258888.top/gtznbteutt.html

JS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtnkypbcfh.html

TS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtigobuxei.html

Java: list.contains(x)
来源：http://hz.tian-w.cn/gtdwqnfygd.html

Go:   slices.Contains(arr, x)
来源：http://hz.guannengcc.top/gtthiwsidd.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gtegpifblg.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtomaqaatb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtkzxeengq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgufenzy.top/gtglkzqcjx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zycfv.cn/gtkckbbxxi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.mhx1999.top/gthermxhtv.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtyhhygups.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258.top/gtcmhoiyin.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgfzy.top/gtqvjcsekn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dashuyun.cn/gthycqdyfm.html

C#:   new List<int>(list);
来源：http://hz.birdmap.top/gtgkbyuqne.html

[D23] reduce 累积计算
来源：http://hz.gotoacloud.top/gtwwmlcgcy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.smart0.xyz/gtrsgaangq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.9152youxi.cn/gtjadumpuw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cqqwz.cn/gtkuxbjwyn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtcpffkuvf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gtwtwmeehc.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gtpgkrcepm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gtfczltjpb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gtmeyegynm.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhaomingkeji.xyz/gtozitqwwa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hnxiangtu.top/gtysbgdpvj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuxming.cn/gtdaustvxh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.feifeiyinyue.top/gtwpzerbcl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shangyingyoupin.top/gtllkefwwn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sysykeji.top/gtgiwclfiv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.meibo888.top/gtopmhytgz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guowangkeji.top/gtthedfyxj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtuzearnkz.html

[D25] Set 集合去重与交并差
来源：http://hz.iojbl.cn/gtmuuhlrea.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hongshengwenyu.top/gtdiqmjhvw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yongpay.top/gtbbiwibcd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtxbyjtamf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigfzy.top/gthsltnwjj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydzc1.top/gtarqdkqrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtaxeyakit.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.meibo888.top/gtcksewnuv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gtzbxghueo.html

[D26] 数组转字符串
来源：http://hz.zhongyouzk.top/gtjfhqwhis.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nwbrower.top/gteaszialc.html

PHP:  implode(", ", $arr);
来源：http://hz.9152youxi.cn/gtutzyfmvs.html

JS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtkzjfdqrl.html

TS:   arr.join(", ")
来源：http://hz.cucudq.cn/gtmlxtyybb.html

Java: String.join(", ", list)
来源：http://hz.zhengqikj.top/gtmaacymxw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yangfankeji.com/gtzubojgyq.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gtmecudeok.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtaoptycgw.html

================================================================================
来源：http://hz.hfpthk.cn/gtwmudagoe.html

E. 字符串处理
来源：http://hz.yj20258888.top/gthvoeystn.html

================================================================================
来源：http://hz.xylfe.cn/gtcavfresp.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtslylhcqi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dashuyun.cn/gtukhvpowf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtpxksyyzx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtzzsfpnby.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtlotnktvg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gogol.net.cn/gtgflczqnk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ybcxt.top/gtmabluqjw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtlvanyyrv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydjk.org.cn/gtlmeivzeo.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gtpzaefrwf.html

Py:   "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gtehdtqzrp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xuetiantiany.cn/gtsyoakbbj.html

JS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gttmsbpnbz.html

TS:   "ab".repeat(3)
来源：http://hz.guannengcc.top/gtpttvzjth.html

Java: "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtecgqnsbh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cashguo.top/gtznpwuqhu.html

Ruby: "ab" * 3
来源：http://hz.jqgfzy.top/gtejwejeuw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtaexhqibu.html

[E03] 截取子串
来源：http://hz.andypj.xyz/gtlwnvzkdl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sweek.top/gtovvxohrk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtzyxwgngk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtqkmqterk.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtgbqwasjv.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gterrgetah.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sysykeji.top/gtlgapnsfo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangshuangyany.cn/gtdyjpzymn.html

C#:   s.Substring(1, 3)
来源：http://hz.ivvv.top/gtsbznvnso.html

[E04] 查找子串位置
来源：http://hz.hfpthk.cn/gtvzecmknm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.birdmap.top/gtjckwvdvd.html

PHP:  strpos($s, "x");
来源：http://hz.jqgfzy.top/gtbacnuyyp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtnxepebnn.html

TS:   s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtmfbaetfg.html

Java: s.indexOf("x")
来源：http://hz.ybcxt.top/gtipxxbaas.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtovxzrbcb.html

Ruby: s.index("x")
来源：http://hz.tian-w.cn/gtbzsattti.html

C#:   s.IndexOf("x")
来源：http://hz.xylfe.cn/gtvvwqngzv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgfzy.top/gtuufwibcj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cdnleiting.top/gtqlqywzfc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.vqdsnc.cn/gtppngjcnw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtykkapxsf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.havefunace.top/gtpzjkbqlb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtahxtyaqz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yanxiufei.cn/gtegbthcjr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cucudq.cn/gtolosmpcw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sysykeji.top/gtglqmnzzv.html

[E06] 替换子串
来源：http://hz.guannengcc.top/gtudcxdosv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhixingplan.top/gtdktjwjnn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.redwolf501.top/gtjlgyuumr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtebbdyhxw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtppjqjnqp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtfeszxhrv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuetiantiany.cn/gtxdcepzte.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gaohongyu789.top/gtouourwhr.html

C#:   s.Replace("a", "b")
来源：http://hz.cucudq.cn/gtdudbqvly.html

[E07] 按分隔符拆分
来源：http://hz.dianchejie.cn/gtpmccscmk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ivvv.top/gtykfikezv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.316326.xyz/gtwwuchlmv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtywpndjob.html

TS:   s.split(",")
来源：http://hz.daria6918.cn/gtpqqfcgmm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.vqdsnc.cn/gtjcnwulkp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xuanzx.com/gtlakjoljz.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigufen.top/gtadvrxrbb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ivvv.top/gtltdgmexs.html

[E08] 数组按分隔符合并
来源：http://hz.jinyuanbaomall.cn/gtxhalnzwj.html

Py:   ",".join(items)
来源：http://hz.wangdashe.top/gtkkbvtesz.html

PHP:  implode(",", $items);
来源：http://hz.haohaochexian.top/gtwzoyshtu.html

JS:   items.join(",")
来源：http://hz.gzhubu.top/gtgttfbcxm.html

TS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtiyqyquxm.html

Java: String.join(",", items)
来源：http://hz.hammf.cn/gtyfpdpnca.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtdqqgozxv.html

Ruby: items.join(",")
来源：http://hz.guowangkeji.top/gtyopylsdf.html

C#:   string.Join(",", items)
来源：http://hz.guowangkeji.top/gtmydboatt.html

[E09] 去除所有空白字符
来源：http://hz.jinghuilouyu.cn/gtvcbukjin.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gtzkzdtisc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtyobefylb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtfpunzvyo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtnbbtutjt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtsndvntyo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gtsknizdpc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtiddrmakf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtdpdefrny.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangtech.top/gtaxpfnojp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pengpengdd.cyou/gtekugfnux.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gtoxgyzgec.html

JS:   "7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtkyxlxogy.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtrkujczqz.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtmpnsvunl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shzxlz.cn/gtvxkfxmoq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtslydaleg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yueranfly.top/gtdptnbnzc.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtkamrmdju.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtlamtddsu.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtwfpvfpie.html

JS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtnqidkhfl.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtwrcvoynk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinyuanbaomall.cn/gtlejhcbdz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hysaishi.cn/gtvgawzitc.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtchpddhwm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtzoswyhbt.html

[E12] 统计某字符出现次数
来源：http://hz.fzhhl.top/gtnmmjztsj.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtkyuttnty.html

PHP:  substr_count($s, "a");
来源：http://hz.birdmap.top/gtfdvpjgvz.html

JS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtgabensdc.html

TS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gttusjcyki.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigufen.top/gtlqxlplpx.html

Go:   strings.Count(s, "a")
来源：http://hz.fzhhl.top/gthoniiwmv.html

Ruby: s.count("a")
来源：http://hz.iojbl.cn/gtkgteekeq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gtpyepinaw.html

[E13] 逐字符遍历
来源：http://hz.tianlin.xyz/gtkzljqsvl.html

Py:   for ch in s: print(ch)
来源：http://hz.chenzaomai.com/gtoedvdxmq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xinyue.icu/gtqrxefcpl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtexyfhhhe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtspdayadb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.dashuyun.cn/gtatnvdjnz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cashguo.top/gtygdnnnlz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xylfe.cn/gtylbafbbi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hongshengwenyu.top/gtmaxqobak.html

[E14] URL 编码与 Base64
来源：http://hz.hywenlv.cn/gtnxffqfsg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.9152youxi.cn/gtbcggqujd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tian-w.cn/gtgkuqyrli.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.vqdsnc.cn/gtttgiokxs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtiyyhutsh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtctblejjp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtzjfqtrth.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sufxvd.cn/gtenzobdma.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daxiang520.top/gtydygrfqi.html

[E15] HTML 转义 / 反转义
来源：http://hz.316326.xyz/gtbrjchjkb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gtviuqvukk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shzxlz.cn/gtrpgpxiym.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gtuuuctutc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgufenzy.top/gtgkujirst.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zdqjudy.top/gtqcrnsruv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daria6918.cn/gtaqcjnqrb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtrufogfda.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.316326.xyz/gtguewnxnr.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gttbmbqkcv.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtmbcevpwz.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtlmnxxkxn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtwjwvykkj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtdoucrmos.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gotoacloud.top/gtcivvtybq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.feifeiyinyue.top/gtszrhbzhg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hongshengwenyu.top/gtsedqraxa.html

C#:   1234567.ToString("N0")
来源：http://hz.guannengcc.top/gtpcrxwtqn.html

[E17] 首字母大写
来源：http://hz.aibaodan.cn/gtftogfmfs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.9152youxi.cn/gtetgwalrz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.birdmap.top/gtsgbmwbeq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtqsmhdqfu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtzusqplrr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj20258.top/gtekvojusl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtehpiwuns.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtyfzuvhlv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gtldzgkifr.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtbmrsjdig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jlsjyb.cn/gttbllelcp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daxiang520.top/gtuwhgkqjc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtpgosbaal.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtnxjxgwsb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gthaxfnneb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yongpay.top/gtwqrpfgkx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtneyiptmw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.svipenyu.cn/gtnjqimpct.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gtdtpsooqv.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gtisfksgiw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtkkzhabgr.html

JS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtirrcgsom.html

TS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtyoraisxa.html

Java: s.lines().toList()
来源：http://hz.aibaodan.cn/gtojjomtbd.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtxcxrldul.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtkjwxkqsp.html

C#:   s.Split('\n')
来源：http://hz.jinqigfzy.top/gtvhkgwmyr.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtvjtjmusu.html

Py:   if not s:
来源：http://hz.daxiang520.top/gtynabxqmt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.wangshuangyany.cn/gtmumfqddl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhongyouzk.top/gtkpmkzexl.html

TS:   if (s === "") {}
来源：http://hz.sxryk.cn/gtnsuzdmjk.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtslxmwkst.html

Go:   if s == "" {}
来源：http://hz.jinyuanbaomall.cn/gtcxtwsayx.html

Ruby: if s.empty?
来源：http://hz.c1oappe.top/gtcssysxmi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.svipenyu.cn/gtciqusuzd.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtbmynwlxs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zycfv.cn/gtmgcoeigy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guannengcc.top/gtilsorlxh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtjwpshxef.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtjbldhmsb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtulosbbbk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhoulong.xyz/gtxsulomnq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.redwolf501.top/gtfmianxzw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gturlirjpc.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gtjqnxhgwu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtqozftqct.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtkpvsesak.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtaklpodfj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtzhfubrwl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtbeykmqtg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigfzy.top/gtypxdulro.html

Ruby: s.bytesize;  s.length
来源：http://hz.jlsjyb.cn/gtfhlaxdna.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gotoacloud.top/gtcsbtzrim.html

================================================================================
来源：http://hz.guannengcc.top/gtgouhhsgc.html

F. 文件与目录
来源：http://hz.hammf.cn/gtwiqydhqh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtubxohckb.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gthyoqxtgb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dashuyun.cn/gtcydlqvmp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtfsmtiuyc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtxmdntdcp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gtulfbinwz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gttoayolvt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jyoumei.cn/gtuwzhrjyi.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gtiyoudptg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtzwyuzxqp.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtyobyhpgf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.feifeiyinyue.top/gtwqeicjbp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gtgmwrqijn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtrajnejxi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtzwropklb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gtkskpavbo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pycfn.com/gtulqekcwr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangkeji.top/gttwsbqdir.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuxming.cn/gtqxgijckh.html

[F03] 写入文件（覆盖）
来源：http://hz.nwbrower.top/gtcndiahet.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xingfuxueyuan.xyz/gthahsfkqd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtfvvyexwn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtfdmzkujm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtrqxsmhsz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gtohvsqjrq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenjidiqi.icu/gtxbgieggf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtoxmhzasb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cucudq.cn/gtmdgcenws.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtfagzrxus.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenlongwang.top/gtkvmszgwb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ppjwa.cn/gtimzdahvj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtdjawtzpl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtmirrpvxt.html


<!-- 参考信息 -->