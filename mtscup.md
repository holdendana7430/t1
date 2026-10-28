代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.xingfuxueyuan.xyz/gtwlldaatz.html

[D16] 求和与平均值
来源：http://hz.yuxming.cn/gtavmxpyxt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtdhghpubf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yueranfly.top/gtzqoqgeet.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gttaszjpyu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenjidiqi.icu/gtnpenwoeb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.bjfxy.top/gtzmtgciaq.html

Go:   // 手写循环累加
来源：http://hz.cheryme.top/gtznznxkak.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtiwzhehim.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtdvwsaxzi.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtfpnpkufp.html

Py:   max(arr);  min(arr)
来源：http://hz.hongshengwenyu.top/gtkqyzexia.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhengqikj.top/gtmsqgkmie.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtyterdhsd.html

TS:   Math.max(...arr);
来源：http://hz.xuetiantiany.cn/gtiqyyzimf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangshuangyany.cn/gtwimwkhfu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtinoyigvu.html

Ruby: arr.max;  arr.min
来源：http://hz.aibaodan.cn/gtijipthmq.html

C#:   list.Max();  list.Min()
来源：http://hz.xuanzx.com/gtgxwfmplg.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtpufcctky.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jiagoushi.top/gtvkrxvpdt.html

PHP:  array_merge(...$nested);
来源：http://hz.yueranfly.top/gtpglgyatl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xylfe.cn/gtychxuakg.html

TS:   nested.flat();
来源：http://hz.cheryme.top/gtzpqnhrcz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.9152youxi.cn/gtuelihene.html

Go:   // 手写双层循环
来源：http://hz.chenzaomai.com/gtanubysvw.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtjqjwubog.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtymhziqlx.html

[D19] 按字段分组
来源：http://hz.yj202588.top/gtzlkiucuk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.kuanghao11.cn/gtghmcclsk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhengqikj.top/gtjjgrnfaz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258.top/gtexeaqhej.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.0kj1m.cn/gtccifhztj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtiksxulgi.html

Go:   // 手写 map[string][]T
来源：http://hz.c1oappe.top/gthtlkqksu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jlsjyb.cn/gthxfphcls.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangshuangyany.cn/gtnuiagmkl.html

[D20] 统计每个元素出现次数
来源：http://hz.zdqjudy.top/gtvmxvkpzy.html

Py:   Counter(arr)
来源：http://hz.hnxiangtu.top/gtsbnefngo.html

PHP:  array_count_values($arr);
来源：http://hz.316326.xyz/gtwgoywlnz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtpvwzjien.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtemnomvua.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhengqikj.top/gtkjqklcsl.html

Go:   // 手写 map[T]int
来源：http://hz.jinghuilouyu.cn/gtokerzohy.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gtarkopxab.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtbamshtiz.html

[D21] 判断是否包含某元素
来源：http://hz.havefunace.top/gtbvybllbo.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtavgdqpnb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hywenlv.cn/gtopvcjayv.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtiuhonssf.html

TS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtaouvlovc.html

Java: list.contains(x)
来源：http://hz.xuetiantiany.cn/gtuaapkzdo.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgfzy.top/gtlpwcnvqy.html

Ruby: arr.include?(x)
来源：http://hz.kuanghao11.cn/gtfhqiyqwf.html

C#:   list.Contains(x)
来源：http://hz.jlsjyb.cn/gtgzvysvhj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daxiang520.top/gtaroxveym.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cdnleiting.top/gtnqgcrpcr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.dashuyun.cn/gtojwoxefo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnxiangtu.top/gtrkdxmhba.html

TS:   [...arr];
来源：http://hz.zhoulong.xyz/gtptjlfqqd.html

Java: new ArrayList<>(list);
来源：http://hz.zdqjudy.top/gtznxejknf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydzc1.top/gtqgucehfq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangshuangyany.cn/gtkosopwge.html

C#:   new List<int>(list);
来源：http://hz.jqgfzy.top/gtydvipxmh.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtygzixrwd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zycfv.cn/gttrmduovi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.mhx1999.top/gtlsfczsyr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtkhlhcgdc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtjvdqriyh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yueranfly.top/gtjhzatjmj.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtizmjlsou.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gtiygwgzgo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhixingplan.top/gtqeqlengs.html

[D24] 字典 / Map 基本操作
来源：http://hz.xinyue.icu/gtoghcjtcx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangshuangyany.cn/gtkmpcwjov.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtxdpcqfwx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.redwolf501.top/gtbrsmursl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yanxiufei.cn/gtvcodqfzb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hysaishi.cn/gtmpvzmwrt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.feifeiyinyue.top/gtfdeucxdi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtfjoaoiao.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sweek.top/gtgkvkbohv.html

[D25] Set 集合去重与交并差
来源：http://hz.ywan-chungtsiang.top/gtpnpgljgn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtgccgniru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aibaodan.cn/gtvzqscrbn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gthxpgerfi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yonumen.top/gtcbwvmoaz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aizwys.cn/gtskfavjia.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtquvanhco.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangtech.top/gtshqqlnxk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydjk.org.cn/gteekwgpuh.html

[D26] 数组转字符串
来源：http://hz.jianghu66.top/gttzpoaugu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.snrcjt.cn/gtfrdbctts.html

PHP:  implode(", ", $arr);
来源：http://hz.zhixingplan.top/gtrxczkxpo.html

JS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtaxrxyouw.html

TS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtlcdgqgkd.html

Java: String.join(", ", list)
来源：http://hz.zdqjudy.top/gtmbwdvmbs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhongyouzk.top/gtshufagxl.html

Ruby: arr.join(", ")
来源：http://hz.guannengcc.top/gtjbmvvsmo.html

C#:   string.Join(", ", list)
来源：http://hz.cucudq.cn/gthqknraqe.html

================================================================================
来源：http://hz.yonumen.top/gtkgpwbmxm.html

E. 字符串处理
来源：http://hz.yvedp.cn/gtypoulhrx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtrtvpmrts.html

[E01] 拼接字符串
来源：http://hz.guannengcc.top/gtjunpfzcp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gaohongyu789.top/gtpdhehomh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhaomingkeji.xyz/gtxyhnocza.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtuhlaseii.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtqfdvegmt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xuanzx.com/gtrepsmexx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gtmqxgvkua.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.52xcode.cn/gtajifvpoh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtpvbndoga.html

[E02] 重复字符串
来源：http://hz.ydzc1.top/gtgjqsbxob.html

Py:   "ab" * 3
来源：http://hz.c1oappe.top/gttxukdqtl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hfpthk.cn/gtdxomfmyy.html

JS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtzbmtefkb.html

TS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtbullxsqt.html

Java: "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtiulqztfc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhaomingkeji.xyz/gtmlnwchfh.html

Ruby: "ab" * 3
来源：http://hz.52xcode.cn/gtdhjotlqt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xylfe.cn/gtmluudgku.html

[E03] 截取子串
来源：http://hz.c1oappe.top/gtlkrlvgot.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtvoyiulsn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtyriglaga.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shuidangran.top/gthkpcbgrw.html

TS:   s.slice(1, 4)
来源：http://hz.fzhhl.top/gtasjvgnbv.html

Java: s.substring(1, 4)
来源：http://hz.yongpay.top/gtvhsjedbf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.vqdsnc.cn/gtclhdkvwd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jyoumei.cn/gthvfmsmpw.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gtwpdnuzbt.html

[E04] 查找子串位置
来源：http://hz.zhaomingkeji.xyz/gtokzkjmfe.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtixroafzs.html

PHP:  strpos($s, "x");
来源：http://hz.svipenyu.cn/gtrsklvfyi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jianghu66.top/gtqwsblnmd.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gticdotweo.html

Java: s.indexOf("x")
来源：http://hz.ehwqpu.com/gturzxzgwg.html

Go:   strings.Index(s, "x")
来源：http://hz.zhiwuduotai.top/gttgxgoidk.html

Ruby: s.index("x")
来源：http://hz.sysykeji.top/gtnirkjddp.html

C#:   s.IndexOf("x")
来源：http://hz.feifeiyinyue.top/gtqisfggls.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.quarkkingdee.top/gtrlqmesnv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cashguo.top/gtqagtlles.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yuanzhike.top/gtygfokbod.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtzimkclah.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gtawvuhfsv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtcezkvfoy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.316326.xyz/gtjliqutvl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuanzhike.top/gtttbuxvqz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ywan-chungtsiang.top/gtuibvdtct.html

[E06] 替换子串
来源：http://hz.xingfuxueyuan.xyz/gtidzorcxc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxinkj.top/gtjgfextjp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guowangkeji.top/gtqldjrqzk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtrvaikutv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtjfjfcqqd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtmozltgxb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yvedp.cn/gtfciywpvp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cdnleiting.top/gtbxoamepn.html

C#:   s.Replace("a", "b")
来源：http://hz.jinghuilouyu.cn/gtzpbfcblf.html

[E07] 按分隔符拆分
来源：http://hz.havefunace.top/gtkxedmkjg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258888.top/gthdrxznlp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aizwys.cn/gtsesllsqh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sufxvd.cn/gtqjagecem.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtdojipwge.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigufen.top/gtaifblnik.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ehwqpu.com/gtqhrbzfbh.html

Ruby: s.split(",");  s.split
来源：http://hz.xinyue.icu/gtzkfhldsj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yonumen.top/gtonltgbqt.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gtpdqyzghr.html

Py:   ",".join(items)
来源：http://hz.haohaochexian.top/gtnniwhzgm.html

PHP:  implode(",", $items);
来源：http://hz.jinqigufen.top/gtzgkipowv.html

JS:   items.join(",")
来源：http://hz.tanke756.top/gtkvzxidtb.html

TS:   items.join(",")
来源：http://hz.bjfxy.top/gtutulcyua.html

Java: String.join(",", items)
来源：http://hz.sxryk.cn/gtueeevlic.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtjixdjrxn.html

Ruby: items.join(",")
来源：http://hz.yj20258.top/gtqlhlvedi.html

C#:   string.Join(",", items)
来源：http://hz.zycfv.cn/gtuvgshszt.html

[E09] 去除所有空白字符
来源：http://hz.chenlongwang.top/gtojqmfcih.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258888.top/gtfbwtozvp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yonumen.top/gtltnlwhsf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtbkefvsnc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtalmgifsz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.mhx1999.top/gtqdmukhhu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangdashe.top/gtjstilgtw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258888.top/gtuodxglje.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtxaoetdvk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dashuyun.cn/gtkhyvpbyl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shzxlz.cn/gtdxddiyto.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhiwuduotai.top/gtmqmjfyqq.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtorglkmwp.html

TS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gttjanlcfe.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtyjfhgnhv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gttpwwaojo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtscddrjqm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ydjk.org.cn/gtkitqetwe.html

[E11] 反转字符串
来源：http://hz.shangyingyoupin.top/gtjbdrmgew.html

Py:   s[::-1]
来源：http://hz.chenlongwang.top/gteliwsbcd.html

PHP:  strrev($s);
来源：http://hz.snrcjt.cn/gtkbxqxmda.html

JS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtealkmhsl.html

TS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtlfgdeams.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtwmwxujes.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinqigfzy.top/gtmqozpfxi.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtsnmwomij.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtgjtzagan.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtzlcuycdv.html

Py:   s.count("a")
来源：http://hz.zhoulong.xyz/gtzcvuwnuf.html

PHP:  substr_count($s, "a");
来源：http://hz.hammf.cn/gttuhtencs.html

JS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtqlvpbbsh.html

TS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtpvztggvu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gtfvouaohx.html

Go:   strings.Count(s, "a")
来源：http://hz.birdmap.top/gtcmsmsgzc.html

Ruby: s.count("a")
来源：http://hz.daxiang520.top/gtsgthkfli.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtxaflpryq.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtcmewvcqq.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtzyloglis.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jiagoushi.top/gtxknsdlmu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtxhxgsefq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtzvkquvea.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.9152youxi.cn/gtsqtjljaw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xylfe.cn/gtdxyykpez.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hammf.cn/gtvfuawvsb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhoulong.xyz/gtxgzfjdoj.html

[E14] URL 编码与 Base64
来源：http://hz.chenjidiqi.icu/gtanyqwsqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtzonibqtj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guannengcc.top/gtmtediiko.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jlsjyb.cn/gttkjkfawd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.316326.xyz/gtnqrwzjka.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sxryk.cn/gtpzgunpqg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtibjsksvw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtxgngkiuk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtsaetphkt.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258888.top/gtxrolvicu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shangyingyoupin.top/gtuwcrcina.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shangyingyoupin.top/gtsyoqjevl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yanxiufei.cn/gtqavhogao.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtbgvsahdc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yongpay.top/gtxsmuzcsm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xylfe.cn/gtiszygkbc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cdnleiting.top/gtpkdpvjax.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxuanxn.top/gtorificwy.html

[E16] 数字千分位
来源：http://hz.haohaochexian.top/gtlplzdqtd.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gthlmzrbtv.html

PHP:  number_format(1234567);
来源：http://hz.haohaochexian.top/gtuexndoyn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtdfzchrgj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.9152youxi.cn/gtvxbpsmcz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtqltpklid.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnqzz.top/gtscfaxlqt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtcglhvgsd.html

C#:   1234567.ToString("N0")
来源：http://hz.meibo888.top/gtzilabhzd.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtnjkfnkky.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gotoacloud.top/gtrdxjhxss.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtolcxzymo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangdashe.top/gtjzuosfkn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtfqjeuwlb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gteagrdlpz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gtnuoevqts.html

Ruby: s.capitalize
来源：http://hz.jinqigfzy.top/gtekeodfwd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ydjk.org.cn/gtavuvgcqz.html

[E18] 模板占位符替换
来源：http://hz.yj202588.top/gtgnskkpxx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangshuangyany.cn/gtarrxholk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gtwifobjcu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtvprbifmn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtutkcajqb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gteriinsiy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtjyxgofgu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydjk.org.cn/gthqyuyfeo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxuanxn.top/gtyawmmigk.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtdqmmwwgo.html

Py:   s.splitlines()
来源：http://hz.yj20258.top/gtgscjfdro.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangkeji.top/gtdrxfqgrz.html

JS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtmnpjabzc.html

TS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtftmfogqe.html

Java: s.lines().toList()
来源：http://hz.ydzc1.top/gtmmunstss.html

Go:   strings.Split(s, "\n")
来源：http://hz.yvedp.cn/gtglygwdlx.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtboprohie.html

C#:   s.Split('\n')
来源：http://hz.tian-w.cn/gtmctbwuam.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gtutawfxmg.html

Py:   if not s:
来源：http://hz.hywenlv.cn/gtmgqfpghd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtjtitofba.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtikmdudpf.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtqaopvukn.html

Java: if (s.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtsufsmyrb.html

Go:   if s == "" {}
来源：http://hz.daxiang520.top/gtnrwgmxth.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gtqhvwfmkx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtfgsuomqr.html

[E21] 超长截断加省略号
来源：http://hz.jianghu66.top/gtxeugxnsf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtqedcwwct.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ydjk.org.cn/gtfnuvxtys.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtczuzrmlw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtieubbdsl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtbfcygxzs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ehwqpu.com/gtxiecijav.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pycfn.com/gtsnsvigay.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhixingplan.top/gtbkzpmqlu.html

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtgojdhiej.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.andypj.xyz/gtiwkigmxa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtnaenamdd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cucudq.cn/gteseriqhp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtcpwgfnoa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgufenzy.top/gtgbzrcnll.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtvpurksks.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydjk.org.cn/gtkwzljdan.html


<!-- 参考信息 -->