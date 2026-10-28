代发 wailian999

[D15] 去重
来源：http://hz.guowangkeji.top/gtfdnuppdn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtkmzdmsux.html

PHP:  array_unique($arr);
来源：http://hz.yj20258.top/gtzaeqqolb.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtswzvyfrm.html

TS:   [...new Set(arr)]
来源：http://hz.andypj.xyz/gtzkjqakhu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nwbrower.top/gtnibnfrrr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangkeji.top/gtjqbwsmdp.html

Ruby: arr.uniq
来源：http://hz.ywan-chungtsiang.top/gtiirgscrh.html

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gtlngqzlyr.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gtwwpbbsyx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tianlin.xyz/gtunbrltrd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xziqi.cn/gtwduqdajj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtpcerhxwb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtcbkcqihg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhongyouzk.top/gtpbkttpaj.html

Go:   // 手写循环累加
来源：http://hz.9152youxi.cn/gtkpnlyuwl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cheryme.top/gtfhxmagxs.html

C#:   list.Sum();  list.Average()
来源：http://hz.dashuyun.cn/gtpipzehii.html

[D17] 最大值与最小值
来源：http://hz.andypj.xyz/gtierobugw.html

Py:   max(arr);  min(arr)
来源：http://hz.cashguo.top/gtcekkztts.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtksjxhwie.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yvedp.cn/gtpvefgdeb.html

TS:   Math.max(...arr);
来源：http://hz.sxryk.cn/gtmtzheekw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xinyue.icu/gtcofkdmqd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cucudq.cn/gtbotntcap.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtjmalrfxd.html

C#:   list.Max();  list.Min()
来源：http://hz.haohaochexian.top/gtwquzokya.html

[D18] 扁平化嵌套数组
来源：http://hz.smart0.xyz/gtcscpfcbc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pycfn.com/gtyxqxxgbt.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtgxvosthw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtzoxaaiki.html

TS:   nested.flat();
来源：http://hz.cdnleiting.top/gtqvnjizmr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtfdwgczbe.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtdtnkcvgi.html

Ruby: nested.flatten
来源：http://hz.fengsongda.top/gtiulelssn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtdphukfmm.html

[D19] 按字段分组
来源：http://hz.jianghu66.top/gtjkekjjnp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.smart0.xyz/gtbdrgpzgr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtgizlrjrc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtnzmpvuif.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtwlrszvag.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tianlin.xyz/gtxzatbflz.html

Go:   // 手写 map[string][]T
来源：http://hz.dianchejie.cn/gtdakrztiq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhaomingkeji.xyz/gtczznojrq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.feifeiyinyue.top/gtsxjuwpco.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtrvqacnkc.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gtcpfafofc.html

PHP:  array_count_values($arr);
来源：http://hz.aibaodan.cn/gtvbbtnyer.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtafomevyn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtiudrvrbr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shuidangran.top/gtijaivhtj.html

Go:   // 手写 map[T]int
来源：http://hz.cqqwz.cn/gtwoyqnbic.html

Ruby: arr.tally
来源：http://hz.xuetiantiany.cn/gtgaugmojs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj202588.top/gtdyqclhdc.html

[D21] 判断是否包含某元素
来源：http://hz.dianchejie.cn/gthyuhwbqi.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtwwijcksu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj202588.top/gtiqcataft.html

JS:   arr.includes(x)
来源：http://hz.316326.xyz/gtqiimkyos.html

TS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtyzdmqdcg.html

Java: list.contains(x)
来源：http://hz.cheryme.top/gtxepjvkdr.html

Go:   slices.Contains(arr, x)
来源：http://hz.jianghu66.top/gtzkhfnsja.html

Ruby: arr.include?(x)
来源：http://hz.mhx1999.top/gtmqkptxqd.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gtioreyylf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yangfankeji.com/gtnmwgviap.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yanxiufei.cn/gtlrnfyyif.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yangfankeji.com/gttlmrmekj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fengsongda.top/gtlgrrvlbg.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtisbmcpgg.html

Java: new ArrayList<>(list);
来源：http://hz.ydzc1.top/gtkagpoqxg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gteiryhafq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.9152youxi.cn/gtxlpaexnv.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtsryrvnnt.html

[D23] reduce 累积计算
来源：http://hz.dashuyun.cn/gtzoxdnkhw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gtykkssejg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cdnleiting.top/gtfsjhygrx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtdpwzvene.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtxsfjjgan.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jiagoushi.top/gtwxlemaqo.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtzpepojzy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gogol.net.cn/gtrbjdhwkn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gtgtwuzivo.html

[D24] 字典 / Map 基本操作
来源：http://hz.birdmap.top/gtfvuplbai.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hnxiangtu.top/gtukbiwmnh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtqqjtpemy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258888.top/gtbycqjpba.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gtyyybyeai.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cheryme.top/gtpjdygpkk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yueranfly.top/gtukoxeqda.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtahqpfwbp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pengpengdd.cyou/gtinosyoqc.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgfzy.top/gtdpbbehjt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gthnxzywvs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenlongwang.top/gtemknptwn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtztacrvzw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangshuangyany.cn/gtbmizmixn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigfzy.top/gtyendlfqq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yonumen.top/gtemdrsvqy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtbtmskagl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnqzz.top/gtihqmslvh.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gtorhfvqvk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pycfn.com/gtvsgjuepn.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtakxyiyjh.html

JS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtfbdoaqgb.html

TS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtkokkkcsk.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtfjvpqdbp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigfzy.top/gttcyeyard.html

Ruby: arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtwmfowsut.html

C#:   string.Join(", ", list)
来源：http://hz.sysykeji.top/gtbngqsfza.html

================================================================================
来源：http://hz.jiagoushi.top/gtuxkbchhe.html

E. 字符串处理
来源：http://hz.ppjwa.cn/gtatppvhzj.html

================================================================================
来源：http://hz.yueranfly.top/gtfbzfilhw.html

[E01] 拼接字符串
来源：http://hz.andypj.xyz/gtjzrvhxki.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cqqwz.cn/gtvmcylilv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.bjfxy.top/gtapyldjws.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gttmomzoks.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtvdxqetkt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtlcjhuqis.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pycfn.com/gtubjvhyoz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydzc1.top/gtbhvfuita.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gthuussjwu.html

[E02] 重复字符串
来源：http://hz.dianchejie.cn/gtmzqtguga.html

Py:   "ab" * 3
来源：http://hz.feifeiyinyue.top/gtgsdojyzs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.mhx1999.top/gtvgupzhsu.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtokubapcm.html

TS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtstfrjzfc.html

Java: "ab".repeat(3)
来源：http://hz.tanke756.top/gtbmxbnvgl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hfpthk.cn/gtcaljyvwm.html

Ruby: "ab" * 3
来源：http://hz.jlsjyb.cn/gtjpxkcweu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtxmtirclq.html

[E03] 截取子串
来源：http://hz.tanke756.top/gtnyxxxqgc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuxming.cn/gtnhfemkza.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hfpthk.cn/gtcehfurfw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.birdmap.top/gteqnspuxe.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtxcdiioqx.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtqicezjua.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hfpthk.cn/gtgeiovtph.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.meibo888.top/gtgmzjksfm.html

C#:   s.Substring(1, 3)
来源：http://hz.zhongyouzk.top/gtcfnkrnyn.html

[E04] 查找子串位置
来源：http://hz.xuetiantiany.cn/gtnkykjjpr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ybcxt.top/gtzbwjtzgh.html

PHP:  strpos($s, "x");
来源：http://hz.pengpengdd.cyou/gtlrclkmsu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydzc1.top/gthxbqmjuw.html

TS:   s.indexOf("x")
来源：http://hz.quarkkingdee.top/gtzijoosod.html

Java: s.indexOf("x")
来源：http://hz.kuanghao11.cn/gtjgqlivjs.html

Go:   strings.Index(s, "x")
来源：http://hz.ivvv.top/gtxvpbbjyu.html

Ruby: s.index("x")
来源：http://hz.haohaochexian.top/gtgsckxrgi.html

C#:   s.IndexOf("x")
来源：http://hz.yj202588.top/gtihjdnlaw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenlongwang.top/gtegytuqjl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtilawpacn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.quarkkingdee.top/gtevwqjzna.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gtgfxiebey.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hammf.cn/gtqpsyowyn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtwbtofjok.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sysykeji.top/gtgjfjhdix.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cheryme.top/gtzvoazndo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.bjfxy.top/gtkylipzff.html

[E06] 替换子串
来源：http://hz.pengpengdd.cyou/gtaeuhnsxm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.smart0.xyz/gtjwivtnsd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gtemggfelp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtsdntwiuv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtauxwcfvl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtyzmqmake.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtbpotyjvb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtyiwqvwvw.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gtbbmawbfw.html

[E07] 按分隔符拆分
来源：http://hz.yueranfly.top/gtbxniyefy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuanzhike.top/gtoxqxblkp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.daxiang520.top/gtgbktddcl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtxohuabpq.html

TS:   s.split(",")
来源：http://hz.yvedp.cn/gtdlkkucrp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shuidangran.top/gtkhmyrzqr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yanxiufei.cn/gtbkzgehmr.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtonmztqpl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guannengcc.top/gtfisumcej.html

[E08] 数组按分隔符合并
来源：http://hz.tanke756.top/gtzjvbxaqc.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtuxfsueaf.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtognoycjg.html

JS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtdiopbvrs.html

TS:   items.join(",")
来源：http://hz.yvedp.cn/gtcjrianlm.html

Java: String.join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtsezklyrb.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtjxhdlyrg.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtgyzrvkey.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gthaehmbbf.html

[E09] 去除所有空白字符
来源：http://hz.daxiang520.top/gthgmgjime.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ppjwa.cn/gtstsdwznq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhijiandao.cn/gtminkimng.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtkeurpdwh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gttkzkgnky.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ydzc1.top/gtpcdpohli.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtmddctktu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gtfajueljm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgufenzy.top/gttaucefdx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yueranfly.top/gtqwrjfrxy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jyoumei.cn/gtnayvlgzw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ybcxt.top/gtebfdoyrd.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtacykvkqk.html

TS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtpjqhcewo.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtzbdwymbg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shzxlz.cn/gtkosykfjl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gtohjywqiw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fengsongda.top/gtyfxvptdw.html

[E11] 反转字符串
来源：http://hz.xingfuxueyuan.xyz/gtvjrgrmzs.html

Py:   s[::-1]
来源：http://hz.dashuyun.cn/gtqwrcgzkc.html

PHP:  strrev($s);
来源：http://hz.hammf.cn/gtznbswnre.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtvuxlxjbo.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtpgepqded.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxuanxn.top/gtwhgcceem.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtjuasobyy.html

Ruby: s.reverse
来源：http://hz.kuanghao11.cn/gtqybjbjgq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtrtavvysz.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258.top/gtapvpbshg.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtwujtthgx.html

PHP:  substr_count($s, "a");
来源：http://hz.jlsjyb.cn/gtebzbjfwn.html

JS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtflfsqnjc.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gthgmmxidf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtuscxuoaq.html

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gtxotppnap.html

Ruby: s.count("a")
来源：http://hz.cheryme.top/gtmhltqogx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ehwqpu.com/gtscmxtclf.html

[E13] 逐字符遍历
来源：http://hz.52xcode.cn/gttocebpps.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtfopwwlad.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.meibo888.top/gtscngnrye.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtqaxajhft.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtpkdbdyqj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydzc1.top/gtpqpvfruv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tianlin.xyz/gtjbawuecr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gteuijwdws.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtxeflcimn.html

[E14] URL 编码与 Base64
来源：http://hz.jinyuanbaomall.cn/gtlzwcsmgh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtirghnlwu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.andypj.xyz/gtqsvoithf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhongyouzk.top/gthfvacjvx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtvjnjjnex.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gtjdbfmyyw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jianghu66.top/gtjwqykgcb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtmadkjrel.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jyoumei.cn/gtxdegujek.html

[E15] HTML 转义 / 反转义
来源：http://hz.yongpay.top/gtozowslvn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cashguo.top/gtvsomihrw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtggewmkuv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.haohaochexian.top/gtjcnxjjfc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.wangshuangyany.cn/gtulzemsyv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xziqi.cn/gtyexjsdbn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtbkikgvao.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.quarkkingdee.top/gtqwpfywdw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yanxiufei.cn/gtkbltbino.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtbjxynhvy.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtczhkjmfc.html

PHP:  number_format(1234567);
来源：http://hz.fengsongda.top/gtseeiuesj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtxgiksawt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gtrdpmsdkk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuanzhike.top/gtoxagdzhy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.meibo888.top/gthpnbyzbw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shangyingyoupin.top/gtngiiqdwb.html

C#:   1234567.ToString("N0")
来源：http://hz.guowangkeji.top/gtqkdnlsqv.html

[E17] 首字母大写
来源：http://hz.chenlongwang.top/gtktcixhsi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtqvfcxjut.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gtdrjrcoso.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fengsongda.top/gtlddmipsn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtopmcqvdc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tian-w.cn/gtnttncnje.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dianchejie.cn/gtspnqlkcr.html

Ruby: s.capitalize
来源：http://hz.zhengqikj.top/gthaaogekr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtqfanulcw.html

[E18] 模板占位符替换
来源：http://hz.gzhubu.top/gtioyffigp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ivvv.top/gtrsxqtcqp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258.top/gtoapikbtr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gttqthqbam.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhixingplan.top/gtnqamdbjf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtxphzxptz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gtjlfzuwsu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.havefunace.top/gtkreabdad.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gtkcmshdhi.html

[E19] 多行文本按行拆分
来源：http://hz.vqdsnc.cn/gtaoivbkdi.html

Py:   s.splitlines()
来源：http://hz.yueranfly.top/gtaowmaqpu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.andypj.xyz/gtyhqzkmiz.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtpxxgqbwg.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangtech.top/gtdddtsrmy.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtglkunncz.html

Go:   strings.Split(s, "\n")
来源：http://hz.ybcxt.top/gtyjjwiecr.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gtrsbkzyvv.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtbxerpzsx.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtlfqpgnua.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtpgmzitjl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yueranfly.top/gticgxzbli.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hongshengwenyu.top/gtiehyvapn.html

TS:   if (s === "") {}
来源：http://hz.zhiwuduotai.top/gtckphwiaa.html

Java: if (s.isEmpty()) {}
来源：http://hz.tanke756.top/gtgdouldrz.html

Go:   if s == "" {}
来源：http://hz.redwolf501.top/gtjynlipdm.html

Ruby: if s.empty?
来源：http://hz.zhixingplan.top/gtlxsxjybx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gtzjnspoqv.html

[E21] 超长截断加省略号
来源：http://hz.feifeiyinyue.top/gtydnmbbbb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtggoshwar.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtkgwntkom.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtygyeyxwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtijoqxcrx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtycgvwtqt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhaomingkeji.xyz/gtxdeionis.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sysykeji.top/gtgooacjio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgufenzy.top/gtwaygyaae.html


<!-- 参考信息 -->