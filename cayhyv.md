代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.svipenyu.cn/gtkyuptbud.html

PHP:  array_merge(...$nested);
来源：http://hz.pycfn.com/gtmgeiagoc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shangyingyoupin.top/gtjvwmcwec.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtgbgtmcko.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgfzy.top/gtbjuhmxdc.html

Go:   // 手写双层循环
来源：http://hz.pycfn.com/gtvmttnutd.html

Ruby: nested.flatten
来源：http://hz.nanxuanxn.top/gtfnuonxka.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuxming.cn/gtqxkcpmiy.html

[D19] 按字段分组
来源：http://hz.jinghuilouyu.cn/gtjkdsoclt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hongshengwenyu.top/gtdxoyevhl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.c1oappe.top/gtxlsiweaw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtikpqaqgw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtlrogqncy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangtech.top/gtmshrqfru.html

Go:   // 手写 map[string][]T
来源：http://hz.daria6918.cn/gtufrfiyfa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtyjutlbnw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtgrqxvxcw.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtozrqzzfv.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangtech.top/gtyqicgpuf.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtpzzjglbr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtgqmvkvew.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtvmpafqxk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtmxrzkywi.html

Go:   // 手写 map[T]int
来源：http://hz.hysaishi.cn/gtyvbyaong.html

Ruby: arr.tally
来源：http://hz.316326.xyz/gtrsxhndvv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gtijjxwnzr.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gthvuwtcza.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtnugdrklb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hammf.cn/gtabgbwbpm.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtcugqmycm.html

TS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtiswqisce.html

Java: list.contains(x)
来源：http://hz.cashguo.top/gthsrdsobi.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtvwzrtovs.html

Ruby: arr.include?(x)
来源：http://hz.zycfv.cn/gtilriavot.html

C#:   list.Contains(x)
来源：http://hz.aibaodan.cn/gtxeyawmiv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.feifeiyinyue.top/gtlxdzmxjl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sufxvd.cn/gtvgbdjpuk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtoielidfn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gtumqlvlmk.html

TS:   [...arr];
来源：http://hz.feifeiyinyue.top/gtpqamnntm.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gtgqqefvla.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtdpqvasnt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydzc1.top/gtvcbetagx.html

C#:   new List<int>(list);
来源：http://hz.yj20258888.top/gtgfhdatsy.html

[D23] reduce 累积计算
来源：http://hz.yuxming.cn/gtddskdoda.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yvedp.cn/gtkmfsihlm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtqgvsjlyt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtacspdbud.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gteuwpqhqv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zycfv.cn/gtqqjowppa.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtboyhuunr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenjidiqi.icu/gtzdbfxhjn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.snrcjt.cn/gtlbhswmdt.html

[D24] 字典 / Map 基本操作
来源：http://hz.jyoumei.cn/gtbujzjqdu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxuanxn.top/gtedpbrnwu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yangfankeji.com/gtvtxvgyhi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydjk.org.cn/gtnmhrnhzy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangtech.top/gthfugwqgi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtwabaaeui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xziqi.cn/gtpxqswnhm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.svipenyu.cn/gtvhjhgqbc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangdashe.top/gtcfxirnid.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtyrzomeom.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtazdwpweh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cqqwz.cn/gtymnlyhzi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zdqjudy.top/gtsjwpwogj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhijiandao.cn/gttetwnbus.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gttoqwjmbg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gotoacloud.top/gtwctqnpcz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shuidangran.top/gtrdrlfzcd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.guowangkeji.top/gtalwwpjsv.html

[D26] 数组转字符串
来源：http://hz.sxryk.cn/gtsqqymhtt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.bjfxy.top/gtuatdsgmq.html

PHP:  implode(", ", $arr);
来源：http://hz.9152youxi.cn/gtxromjutn.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtgtggahve.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtcfxvpzkb.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtflogache.html

Go:   strings.Join(strs, ", ")
来源：http://hz.snrcjt.cn/gtymjjbnxk.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gthrlddalt.html

C#:   string.Join(", ", list)
来源：http://hz.cdnleiting.top/gtuibkzcbu.html

================================================================================
来源：http://hz.hywenlv.cn/gtpndlmgej.html

E. 字符串处理
来源：http://hz.shanyushiyangtech.top/gtxwrtagpn.html

================================================================================
来源：http://hz.zdqjudy.top/gtpgmfdxeo.html

[E01] 拼接字符串
来源：http://hz.hammf.cn/gtkyqdbuwj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtgykbhune.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.316326.xyz/gtbuhpkgxt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtijznthdv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtcxvdqrsw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cashguo.top/gtassirdpr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj202588.top/gtxmcuazkn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nwbrower.top/gtuqsrsdxs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gtxqrtngyn.html

[E02] 重复字符串
来源：http://hz.ehwqpu.com/gtlisbcbxo.html

Py:   "ab" * 3
来源：http://hz.guowangkeji.top/gtlgvnbaup.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ehwqpu.com/gtrkkhyzmn.html

JS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtcfvcsttn.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtqqkmtbhz.html

Java: "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtjunlngpi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hysaishi.cn/gtvalpwoyp.html

Ruby: "ab" * 3
来源：http://hz.pycfn.com/gtuejzwsxz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tianlin.xyz/gtupbhsajl.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gteferhmvw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pycfn.com/gtnlbcfoqr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtzryaluhw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtyujahvkl.html

TS:   s.slice(1, 4)
来源：http://hz.sysykeji.top/gttshwbsut.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gteaxbaabj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gtaptaxuel.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yongpay.top/gtwnhddsjr.html

C#:   s.Substring(1, 3)
来源：http://hz.yuxming.cn/gtghxtvrip.html

[E04] 查找子串位置
来源：http://hz.ybcxt.top/gtotwhqyhq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhoulong.xyz/gtfkcetvcq.html

PHP:  strpos($s, "x");
来源：http://hz.sxryk.cn/gtufotdoch.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jianghu66.top/gtjisboojd.html

TS:   s.indexOf("x")
来源：http://hz.cheryme.top/gtusgglorq.html

Java: s.indexOf("x")
来源：http://hz.yueranfly.top/gtkqofbxjh.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtdsvmwvxo.html

Ruby: s.index("x")
来源：http://hz.52xcode.cn/gtnntzuzto.html

C#:   s.IndexOf("x")
来源：http://hz.yueranfly.top/gtszomalpa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtgulzftvs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenlongwang.top/gtyjspobmf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydjk.org.cn/gtrofhqczy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtvwwljdah.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xuetiantiany.cn/gtvubjzhua.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtlhoxxwzf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gaohongyu789.top/gtaedafnbf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenzaomai.com/gtdlgtxqcu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ybcxt.top/gtjswmtjsw.html

[E06] 替换子串
来源：http://hz.yonumen.top/gtarnebvkl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dianchejie.cn/gtpippcgre.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xingfuxueyuan.xyz/gtpfpugjps.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtsdbxcyjb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtiqpxgkve.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtceugjsbn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yangfankeji.com/gteevcmiya.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hammf.cn/gttnzgazuw.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgfzy.top/gtfjzyhxas.html

[E07] 按分隔符拆分
来源：http://hz.feifeiyinyue.top/gtsfhphstr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigfzy.top/gtwqwbshjr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guannengcc.top/gtcvnxexjn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sxryk.cn/gtpqxvdjkr.html

TS:   s.split(",")
来源：http://hz.zhiwuduotai.top/gthdzhsiis.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.c1oappe.top/gthpaqhcyw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hammf.cn/gtrhipxuoo.html

Ruby: s.split(",");  s.split
来源：http://hz.tanke756.top/gtxitcjtqe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtyijgqwwd.html

[E08] 数组按分隔符合并
来源：http://hz.birdmap.top/gtcpcpfuqq.html

Py:   ",".join(items)
来源：http://hz.jlsjyb.cn/gtismkluso.html

PHP:  implode(",", $items);
来源：http://hz.yj20258.top/gtsfapthra.html

JS:   items.join(",")
来源：http://hz.yuxming.cn/gtfavvyaid.html

TS:   items.join(",")
来源：http://hz.ivvv.top/gtcusiqmjx.html

Java: String.join(",", items)
来源：http://hz.jyoumei.cn/gtutmpxvhn.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtdofuoxdf.html

Ruby: items.join(",")
来源：http://hz.cashguo.top/gtcqyvmyem.html

C#:   string.Join(",", items)
来源：http://hz.sufxvd.cn/gtqzqqlpwe.html

[E09] 去除所有空白字符
来源：http://hz.sxryk.cn/gtfbswmsmx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dashuyun.cn/gtrgnmmezi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gtzumforxh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtepzkvxbp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtpbuxgceg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.birdmap.top/gtndpqszbp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtxkljlvub.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sxryk.cn/gtnztuawdi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gtjynzoxjy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.meibo888.top/gtwlcxvmpm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj202588.top/gtuozrgwuu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hammf.cn/gtkxrvhgaz.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtawfbcvgt.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtrcmospmn.html

Java: String.format("%03d", 7)
来源：http://hz.jianghu66.top/gtjlvizeum.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gtutmzvhiz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtoaxvifow.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtohzedbkq.html

[E11] 反转字符串
来源：http://hz.zdqjudy.top/gtdrntrkra.html

Py:   s[::-1]
来源：http://hz.shuidangran.top/gtyyjzcifa.html

PHP:  strrev($s);
来源：http://hz.0kj1m.cn/gtjvkutwye.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtlcfbmzkm.html

TS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtisgjvtoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenjidiqi.icu/gtmnznqkox.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258888.top/gtsnxydidx.html

Ruby: s.reverse
来源：http://hz.hongshengwenyu.top/gtarpsucvy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gthlafldfy.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtyaldzilx.html

Py:   s.count("a")
来源：http://hz.xinyue.icu/gtufsxlzif.html

PHP:  substr_count($s, "a");
来源：http://hz.tanke756.top/gtarbjempk.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtkrkfkqei.html

TS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtgbctkynd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtchkinnio.html

Go:   strings.Count(s, "a")
来源：http://hz.kuanghao11.cn/gtujfqdvcf.html

Ruby: s.count("a")
来源：http://hz.ydzc1.top/gtjpertyan.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gtpkvbemnp.html

[E13] 逐字符遍历
来源：http://hz.xylfe.cn/gtrtisdiwv.html

Py:   for ch in s: print(ch)
来源：http://hz.ydjk.org.cn/gthebitbaa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangdashe.top/gtungobotd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtslsfggkg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtmkjlenvv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gttnwcollk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gzhubu.top/gtypoescdd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.haohaochexian.top/gtgloihqrr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtsuumdnbu.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtpjwkiyqo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangkeji.top/gtfzmdtrnc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtdfutgwol.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gtazkgfzkf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gtfnkygeex.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ybcxt.top/gtrthhntkt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigufen.top/gtuubivvct.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtkzptndjp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aizwys.cn/gtseikfesj.html

[E15] HTML 转义 / 反转义
来源：http://hz.yanxiufei.cn/gtjjlegcdw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fzhhl.top/gtjnxlgupe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ybcxt.top/gtuzusskwm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnqzz.top/gtwavkrqbs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jlsjyb.cn/gtglltgucz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ybcxt.top/gtwbrosqdb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aizwys.cn/gtvxgxtzcc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuanzx.com/gtndjnhoca.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.316326.xyz/gttofetwzc.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtepvqnfeo.html

Py:   f"{1234567:,}"
来源：http://hz.meibo888.top/gtcpufnrnc.html

PHP:  number_format(1234567);
来源：http://hz.xylfe.cn/gtslzlopcq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtvbjkfmlk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gttssgjnbh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.vqdsnc.cn/gtbtbotudu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guowangkeji.top/gtewjszvbr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.andypj.xyz/gtxuxbpcbi.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtqdsieiix.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gtblotoqxd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.quarkkingdee.top/gtslmlihcu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuanzx.com/gtltxjmgsv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtjfslclda.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtiatpaftc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgufenzy.top/gtbuprcrch.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hysaishi.cn/gtwpilffik.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtmnwmicay.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nwbrower.top/gtrpumnzvk.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gtqmfukonq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtgtqtolxo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tianlin.xyz/gtxqsbpltu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtgjjuneuf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtcytsvgxw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gtpbxgeqiz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xziqi.cn/gtelluvghg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gtyoxawbks.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuanzx.com/gtlkjbazxq.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtxxvtkqdk.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtpjucxvzp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gtvhhzqdxm.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtgdjihwba.html

TS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtdmmkhkay.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtmvneuyml.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinghuilouyu.cn/gtplglgsfk.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gtysrvjxiw.html

C#:   s.Split('\n')
来源：http://hz.daria6918.cn/gtnuswqitc.html

[E20] 判断字符串是否为空
来源：http://hz.gogol.net.cn/gtrhsrrrqk.html

Py:   if not s:
来源：http://hz.quarkkingdee.top/gtggedlqvb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gtfclhkfkm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtgrbwosag.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtiaclxqbk.html

Java: if (s.isEmpty()) {}
来源：http://hz.ywan-chungtsiang.top/gtkyiwwkkw.html

Go:   if s == "" {}
来源：http://hz.shangyingyoupin.top/gtcuqsfhpu.html

Ruby: if s.empty?
来源：http://hz.jlsjyb.cn/gtguouuwdg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gtvztxyzqb.html

[E21] 超长截断加省略号
来源：http://hz.dashuyun.cn/gtmebdmfei.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuetiantiany.cn/gtfmillhic.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gzhubu.top/gtczhdypai.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtmoxtzqgq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtkwnaapli.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtdcleilau.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigfzy.top/gtfwjkkjjg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xinyue.icu/gtfioaaeza.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtbjzdgmng.html

[E22] 字节长度与字符长度
来源：http://hz.cqqwz.cn/gtujqytktk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yangfankeji.com/gtvwioyeye.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gthdfhzezt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtgcisfrrc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtkmfqchxc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ybcxt.top/gtmzyuyhso.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gthsayybrn.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgfzy.top/gtflghgpku.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtgrortjto.html

================================================================================
来源：http://hz.guannengcc.top/gtuwuobbou.html

F. 文件与目录
来源：http://hz.wangdashe.top/gtbuhdtwbn.html

================================================================================
来源：http://hz.redwolf501.top/gtihmlsvyx.html

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtmawjkjgw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhongyouzk.top/gtwnmbsymq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jyoumei.cn/gtubjkvsbm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtcwjnksob.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gttmamxsfo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtuwsipxna.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sysykeji.top/gtdqvzabic.html

Ruby: File.read("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtunezmprq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hysaishi.cn/gtgmvnhnid.html

[F02] 逐行读取文件
来源：http://hz.mhx1999.top/gtspiknghv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gteecosrfq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.smart0.xyz/gtnhzvdywl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtwvddqxwf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtgddzaouf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtbuzcunnv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigfzy.top/gtvzmjvmmj.html


<!-- 参考信息 -->