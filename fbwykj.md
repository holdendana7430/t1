代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtdoisnynp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtrudolias.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgfzy.top/gtkvmybepi.html

Ruby: arr.uniq
来源：http://hz.zhixingplan.top/gtqrjdjkrj.html

C#:   list.Distinct().ToList()
来源：http://hz.daria6918.cn/gtwikmilmk.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtfmwbnawq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtrjjbbcwr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gtpdxelcud.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtcocwjyya.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtruqkjryr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cdnleiting.top/gticjqsslg.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtmzpokeic.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gtkmciqwbf.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtkthdglzb.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtstquijkf.html

Py:   max(arr);  min(arr)
来源：http://hz.kuanghao11.cn/gtlrjpryck.html

PHP:  max($arr);  min($arr);
来源：http://hz.zycfv.cn/gtzuvyhrnd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.0kj1m.cn/gtscuhjpat.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangtech.top/gtdczbhuhc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.316326.xyz/gtqiyunaiz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuxming.cn/gtmnldbflv.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258888.top/gtqfisijsz.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gtczovtmui.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gtlcayziaa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.c1oappe.top/gtlnjmzdzz.html

PHP:  array_merge(...$nested);
来源：http://hz.svipenyu.cn/gtnuyrhsqv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cqqwz.cn/gtvoyldqyi.html

TS:   nested.flat();
来源：http://hz.sufxvd.cn/gtpczqliwq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.mhx1999.top/gtccngrsbv.html

Go:   // 手写双层循环
来源：http://hz.hfpthk.cn/gtisnlpkbe.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtpgfyxsft.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.316326.xyz/gtiblntuyt.html

[D19] 按字段分组
来源：http://hz.feifeiyinyue.top/gtqmcmivcy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.iojbl.cn/gtvmbzafni.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtnwolzvao.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuxming.cn/gtxblnjukr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtbhmlsxbo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.redwolf501.top/gtasorzmtj.html

Go:   // 手写 map[string][]T
来源：http://hz.hongshengwenyu.top/gtmcahpvkk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hfpthk.cn/gthvigpatw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.guowangkeji.top/gtpxfsdkcs.html

[D20] 统计每个元素出现次数
来源：http://hz.ybcxt.top/gtmjjdmswk.html

Py:   Counter(arr)
来源：http://hz.hnxiangtu.top/gtupjtuqhs.html

PHP:  array_count_values($arr);
来源：http://hz.sufxvd.cn/gtmztntiko.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtrfsdxeyu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gttonsptpr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ywan-chungtsiang.top/gtoekabczu.html

Go:   // 手写 map[T]int
来源：http://hz.zdqjudy.top/gtvelvoztf.html

Ruby: arr.tally
来源：http://hz.jqgfzy.top/gtppwigxvf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sufxvd.cn/gtnanxvdwf.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gtbfiubydk.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtsnzbybvb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cheryme.top/gtcsmjlklc.html

JS:   arr.includes(x)
来源：http://hz.tian-w.cn/gttskizowe.html

TS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtjqjcztfx.html

Java: list.contains(x)
来源：http://hz.vqdsnc.cn/gtphcvaizd.html

Go:   slices.Contains(arr, x)
来源：http://hz.cqqwz.cn/gtudswxmwj.html

Ruby: arr.include?(x)
来源：http://hz.vqdsnc.cn/gtgpypgfav.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtagettgbu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yuanzhike.top/gtcppvwxsb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jiagoushi.top/gtubuhcobh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtcwqrijse.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.feifeiyinyue.top/gtheldevzv.html

TS:   [...arr];
来源：http://hz.tianlin.xyz/gtpnfyyslr.html

Java: new ArrayList<>(list);
来源：http://hz.c1oappe.top/gtraefmvnl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangkeji.top/gtmlenxyfw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aizwys.cn/gtmbfpmtax.html

C#:   new List<int>(list);
来源：http://hz.sysykeji.top/gtsgzezyew.html

[D23] reduce 累积计算
来源：http://hz.52xcode.cn/gtiumdocss.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuanzhike.top/gtavwvrkwy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangtech.top/gtcrjsjxli.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtbttaohlo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtzxabpzod.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenjidiqi.icu/gtphyicnke.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtguqwhioy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xziqi.cn/gtillbwfzs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gtzihwvsgj.html

[D24] 字典 / Map 基本操作
来源：http://hz.shanyushiyangtech.top/gtxyvbjxfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cheryme.top/gtimjxyagx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtxjysrmgp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtridlozzd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.kuanghao11.cn/gtunduxfcg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xinyue.icu/gtaoycjfgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhongyouzk.top/gtjyzkzmhs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtgcohqgja.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gtgiveyqwq.html

[D25] Set 集合去重与交并差
来源：http://hz.guowangkeji.top/gtcjfuzecz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xziqi.cn/gtjmzdpkbs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nwbrower.top/gtryzjguhd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.havefunace.top/gtertiyeno.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hywenlv.cn/gtwsrgppuw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhijiandao.cn/gtytfscwqk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigufen.top/gtqvhzxuvv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aibaodan.cn/gtfrpiofvc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gotoacloud.top/gtkoeykonn.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtxywesiec.html

Py:   ", ".join(map(str, arr))
来源：http://hz.havefunace.top/gtdtmdvnso.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtoxzosrsw.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtztichbpj.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gthmwpozxm.html

Java: String.join(", ", list)
来源：http://hz.hywenlv.cn/gtneelndzq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xziqi.cn/gtpvchpmyd.html

Ruby: arr.join(", ")
来源：http://hz.tianlin.xyz/gtuhaozdpl.html

C#:   string.Join(", ", list)
来源：http://hz.ehwqpu.com/gtekbpsxvx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvlffqsps.html

E. 字符串处理
来源：http://hz.zhixingplan.top/gtisqdxtrv.html

================================================================================
来源：http://hz.jqgfzy.top/gtwmroditf.html

[E01] 拼接字符串
来源：http://hz.jlsjyb.cn/gtjkpjyfpl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtwppqukhe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258888.top/gtyqtuegyh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtteaqgugb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtcpbsgmiu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aibaodan.cn/gtljrfclna.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.52xcode.cn/gtcyqdqlwl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.haohaochexian.top/gtphlxdbic.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ppjwa.cn/gtbftujgsg.html

[E02] 重复字符串
来源：http://hz.hnqzz.top/gticictveg.html

Py:   "ab" * 3
来源：http://hz.jqgufenzy.top/gtouvisvne.html

PHP:  str_repeat("ab", 3);
来源：http://hz.bjfxy.top/gttspnvlyg.html

JS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtsehuvpfp.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtymimpqcr.html

Java: "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtqizzoqun.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pengpengdd.cyou/gtyfpkijwe.html

Ruby: "ab" * 3
来源：http://hz.cashguo.top/gtkbptyaei.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nwbrower.top/gtrlznbpfh.html

[E03] 截取子串
来源：http://hz.hywenlv.cn/gttxdczuii.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hywenlv.cn/gtjbihhybf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jlsjyb.cn/gtevpbgjik.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.316326.xyz/gtwzdawhuc.html

TS:   s.slice(1, 4)
来源：http://hz.aizwys.cn/gtmuliqzpr.html

Java: s.substring(1, 4)
来源：http://hz.smart0.xyz/gtobduioap.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gtqymhfleo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuanzx.com/gtejfufktq.html

C#:   s.Substring(1, 3)
来源：http://hz.9152youxi.cn/gtmnzesutn.html

[E04] 查找子串位置
来源：http://hz.cqqwz.cn/gtyhnftimc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xuetiantiany.cn/gtymjmjvhz.html

PHP:  strpos($s, "x");
来源：http://hz.gzhubu.top/gtcmrakkvu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangshuangyany.cn/gtvavangdx.html

TS:   s.indexOf("x")
来源：http://hz.jqgfzy.top/gtmjwhtnjj.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtnhizdgmf.html

Go:   strings.Index(s, "x")
来源：http://hz.snrcjt.cn/gtpkbbwxmw.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtahplhuxf.html

C#:   s.IndexOf("x")
来源：http://hz.dianchejie.cn/gtmkvumfhw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxuanxn.top/gtjyrlzezo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuetiantiany.cn/gtbwovtatt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.mhx1999.top/gtdqkzixgw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtrtqyeekg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtptodgpzf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtaqjmhgjm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jlsjyb.cn/gtsszoerry.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guannengcc.top/gtdopqeskw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xinyue.icu/gtvypjedoe.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gtrhyjghwj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gotoacloud.top/gtoouiivji.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jiagoushi.top/gtioaaxqdm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtqdhrfqjg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gttrhiplyu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtjqcgpfya.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.redwolf501.top/gtehalyppw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtbiykpbwk.html

C#:   s.Replace("a", "b")
来源：http://hz.daria6918.cn/gtrwzbcxvo.html

[E07] 按分隔符拆分
来源：http://hz.bjfxy.top/gtenoyvjdb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guowangkeji.top/gtgyrnjiay.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gtgzsucrgt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nwbrower.top/gtytvaownd.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtjspniifa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ybcxt.top/gtlybxlccp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.redwolf501.top/gttmwtsdbz.html

Ruby: s.split(",");  s.split
来源：http://hz.jiagoushi.top/gtacamwaps.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jianghu66.top/gtwlgjbjxl.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtrsjoeqol.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtlxzmbgho.html

PHP:  implode(",", $items);
来源：http://hz.cheryme.top/gtigsscfih.html

JS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gttvwpmtek.html

TS:   items.join(",")
来源：http://hz.nanxuanxn.top/gtbnzpxxha.html

Java: String.join(",", items)
来源：http://hz.ydjk.org.cn/gtjkckiaqv.html

Go:   strings.Join(items, ",")
来源：http://hz.jianghu66.top/gtifliykju.html

Ruby: items.join(",")
来源：http://hz.sufxvd.cn/gtuahxkfli.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtogeogcdx.html

[E09] 去除所有空白字符
来源：http://hz.cucudq.cn/gtekpaetkv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtbejslrer.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.bjfxy.top/gtdaezntul.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtvntxzskn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtcukeqais.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aizwys.cn/gtdwclabzp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.meibo888.top/gtdthdztst.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aibaodan.cn/gtxwwlluub.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gthrxsfiwg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jyoumei.cn/gtbcfgqlga.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtsecmnlyk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jqgfzy.top/gtgvqguxsx.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtzoolmupg.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtctlwcjwu.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtytlmmeyz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zycfv.cn/gtrwhcvnic.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtqetdjmsq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.9152youxi.cn/gtwsklktkn.html

[E11] 反转字符串
来源：http://hz.cucudq.cn/gtrhyubsqf.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtorfnbdym.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtjfatkmkk.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtizgxwakw.html

TS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtdwlglqfk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hysaishi.cn/gtisstmrnt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hysaishi.cn/gtjzpjcwpg.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gtjpsevclg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtigtzcywe.html

[E12] 统计某字符出现次数
来源：http://hz.quarkkingdee.top/gticmspcuy.html

Py:   s.count("a")
来源：http://hz.guannengcc.top/gtmnuvuzrm.html

PHP:  substr_count($s, "a");
来源：http://hz.zdqjudy.top/gtknmrcndg.html

JS:   s.split("a").length - 1
来源：http://hz.nanxinkj.top/gtukmypzem.html

TS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtmcdpqcna.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtcqxgsguh.html

Go:   strings.Count(s, "a")
来源：http://hz.yuxming.cn/gthdfgqold.html

Ruby: s.count("a")
来源：http://hz.birdmap.top/gtxuheptpc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinyuanbaomall.cn/gthkienmev.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtfriofpqb.html

Py:   for ch in s: print(ch)
来源：http://hz.fzhhl.top/gtwgdneyas.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guannengcc.top/gtqepqrqoz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gtljjcilhj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtiponcmqv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.kuanghao11.cn/gtqljbjsis.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shzxlz.cn/gttctzzxom.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtaufdgtva.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnqzz.top/gthwjwfkba.html

[E14] URL 编码与 Base64
来源：http://hz.iojbl.cn/gtbobvmchm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtgaycpwrf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jiagoushi.top/gtmnbqezhs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtuzjddizp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gtqblywohf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xziqi.cn/gtqzlgjjov.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sweek.top/gtwtnysoki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtklfktxwt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pycfn.com/gtwtmtwcbs.html

[E15] HTML 转义 / 反转义
来源：http://hz.cdnleiting.top/gttyppcmdk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenjidiqi.icu/gtnnlhmmvk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258888.top/gtkgkvbrvx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cheryme.top/gtazxqazve.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtlefagxdv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtcytxxnea.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.havefunace.top/gtwlrvlzah.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yonumen.top/gtsplrsqiy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtekloigxt.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gtscflfwxz.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gtcxlwnfdr.html

PHP:  number_format(1234567);
来源：http://hz.cqqwz.cn/gtvrkpopbl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtfmbnreub.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtvxoadnkn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yvedp.cn/gthhaircqs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.redwolf501.top/gtrqvplpxj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ywan-chungtsiang.top/gtqtbofcuy.html

C#:   1234567.ToString("N0")
来源：http://hz.yueranfly.top/gtqjuxeiku.html

[E17] 首字母大写
来源：http://hz.shzxlz.cn/gtwytqncmo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxuanxn.top/gtlompobfb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenlongwang.top/gtkenhyaja.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtyiklyxcw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtobobuxxo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtpcnsjqdj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xylfe.cn/gttwqohldn.html

Ruby: s.capitalize
来源：http://hz.aibaodan.cn/gtbvgagqjq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhixingplan.top/gtllksfgkm.html

[E18] 模板占位符替换
来源：http://hz.nwbrower.top/gtguvvlcyf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzhubu.top/gthjuklwmd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ppjwa.cn/gtidddccrz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258888.top/gtxadcczqz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtrwnzyjbw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtxovvbxnn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj202588.top/gtosrvlizu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gogol.net.cn/gtpjdpbmdo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtbkvyvybk.html

[E19] 多行文本按行拆分
来源：http://hz.andypj.xyz/gtooarnisk.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gthytciwyv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dashuyun.cn/gthafxpijc.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gtwpyyodrh.html

TS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtjfjxtarj.html

Java: s.lines().toList()
来源：http://hz.ydzc1.top/gtsngwcgyk.html

Go:   strings.Split(s, "\n")
来源：http://hz.pengpengdd.cyou/gtslopiwri.html

Ruby: s.lines
来源：http://hz.zhoulong.xyz/gtajwfghky.html

C#:   s.Split('\n')
来源：http://hz.gzhubu.top/gtjaftsujo.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gtntswnezw.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gttpnmbkss.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yonumen.top/gtwmoynrgm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pycfn.com/gtndeaipgg.html

TS:   if (s === "") {}
来源：http://hz.hfpthk.cn/gtpgacdirq.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtavoxqhox.html

Go:   if s == "" {}
来源：http://hz.shuidangran.top/gtcvvkiqwl.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtntfqdspw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fzhhl.top/gtreboitup.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gtfqzvdsex.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sxryk.cn/gtjixsklhj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtdkaakxvi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtkijmryey.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtxhmftorc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtmsgkeodl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yueranfly.top/gtjqrdymnf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.havefunace.top/gtysjoklcm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhixingplan.top/gthtzkmnkv.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gtzubedlfn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtpxnylgxd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtsefidfts.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtmushvlmq.html


<!-- 参考信息 -->