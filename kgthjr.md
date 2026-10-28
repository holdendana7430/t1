代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xylfe.cn/gtotawddiw.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtgflfgstt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gtvdxftrdm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tanke756.top/gteghrsqig.html

[D15] 去重
来源：http://hz.hnqzz.top/gtixgerrcs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtrndxoisa.html

PHP:  array_unique($arr);
来源：http://hz.zhiwuduotai.top/gtwedyvteu.html

JS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtzbwhzzjw.html

TS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtpsjnmgog.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sysykeji.top/gticskoqcs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daria6918.cn/gtfnvxmydh.html

Ruby: arr.uniq
来源：http://hz.feifeiyinyue.top/gtccwncpja.html

C#:   list.Distinct().ToList()
来源：http://hz.ivvv.top/gtyzesmate.html

[D16] 求和与平均值
来源：http://hz.9152youxi.cn/gtgbglewtt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yangfankeji.com/gtazvuuacw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtzvfwyecy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxinkj.top/gtoahzwzqy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gthbjneuol.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yangfankeji.com/gtkyyekhfr.html

Go:   // 手写循环累加
来源：http://hz.jqgufenzy.top/gtwipmiinp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gtvsirtmss.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gtajgsglzf.html

[D17] 最大值与最小值
来源：http://hz.shzxlz.cn/gtrxrjkdcf.html

Py:   max(arr);  min(arr)
来源：http://hz.zhijiandao.cn/gtsmfqxzzn.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gtbnfsewoe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zycfv.cn/gtwxuntsna.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtqqtpswwt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gzhubu.top/gtyewubxxz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhijiandao.cn/gtuvxtyohk.html

Ruby: arr.max;  arr.min
来源：http://hz.sxryk.cn/gtqiwtqida.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangkeji.top/gtyzctckro.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtkpybsqsz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtyaoxjrnv.html

PHP:  array_merge(...$nested);
来源：http://hz.kuanghao11.cn/gtiptjjioy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangtech.top/gtjektpimh.html

TS:   nested.flat();
来源：http://hz.hammf.cn/gtiacnoomd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhiwuduotai.top/gtnwxlbagc.html

Go:   // 手写双层循环
来源：http://hz.nanxuanxn.top/gtxbnikjcd.html

Ruby: nested.flatten
来源：http://hz.yongpay.top/gthggcxemy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gogol.net.cn/gtmswbhhio.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtjezwgvho.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cheryme.top/gtaxqtddgl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhijiandao.cn/gtzeoiuogx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtbalexpry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtxcujrgxi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtlnyhpjdt.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtyykeovnf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.iojbl.cn/gtkmgjzung.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aibaodan.cn/gtxpsjesbp.html

[D20] 统计每个元素出现次数
来源：http://hz.xingfuxueyuan.xyz/gthtomciil.html

Py:   Counter(arr)
来源：http://hz.jiagoushi.top/gtlchdcnxd.html

PHP:  array_count_values($arr);
来源：http://hz.wangshuangyany.cn/gtsmaykxbx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtnmyzdfrw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtexhajpyf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.redwolf501.top/gtnrmcuqcg.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gtgbxttscl.html

Ruby: arr.tally
来源：http://hz.nwbrower.top/gteovjooex.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj202588.top/gtndwkzgmg.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtvhxfvgxq.html

Py:   x in arr
来源：http://hz.gotoacloud.top/gttkisapef.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenlongwang.top/gtheqbapoq.html

JS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtyehifmqo.html

TS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtoojwshqx.html

Java: list.contains(x)
来源：http://hz.xuetiantiany.cn/gttebzcllr.html

Go:   slices.Contains(arr, x)
来源：http://hz.yangfankeji.com/gtooajvkhl.html

Ruby: arr.include?(x)
来源：http://hz.hammf.cn/gtzcavinjp.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gttjvzdwim.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sweek.top/gtchatexrb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.birdmap.top/gtfgaeybjb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hfpthk.cn/gtuwhtrnio.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shuidangran.top/gtnhxvnzdh.html

TS:   [...arr];
来源：http://hz.daxiang520.top/gtsyysxglc.html

Java: new ArrayList<>(list);
来源：http://hz.xingfuxueyuan.xyz/gtbiblzkrj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daria6918.cn/gtfogeillr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gthzndrrmb.html

C#:   new List<int>(list);
来源：http://hz.yj20258.top/gtefxcaqlj.html

[D23] reduce 累积计算
来源：http://hz.ydzc1.top/gtvcexoqbv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gthxmjcfwj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangtech.top/gtwgeuzbsg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtjytbspbm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtwftyrnub.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtkrdyrfkw.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtmetgdwqq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.c1oappe.top/gtpekyqxgf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtrsglupbf.html

[D24] 字典 / Map 基本操作
来源：http://hz.cucudq.cn/gtuvbyxzkv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fengsongda.top/gtmyipkikk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangtech.top/gtqbkxvojl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.snrcjt.cn/gtkgpjqyiv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj202588.top/gtxhpwmugq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.feifeiyinyue.top/gtwxxdchdw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dashuyun.cn/gtubumcbht.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hongshengwenyu.top/gtqruqbzzd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.redwolf501.top/gthvjoqknd.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtgxcagnbi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hfpthk.cn/gthvbgwxmn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtdnhamuka.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangdashe.top/gtzvrqxxjr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aibaodan.cn/gtcqdrtblg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtmqzbdyjz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yongpay.top/gtxymyamle.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.svipenyu.cn/gtxlmajxhg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhengqikj.top/gtvypancfw.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gtwgkrdtdl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hammf.cn/gtcomfxaxt.html

PHP:  implode(", ", $arr);
来源：http://hz.xuetiantiany.cn/gtehdiceag.html

JS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtlamaunvr.html

TS:   arr.join(", ")
来源：http://hz.meibo888.top/gtvaurahaj.html

Java: String.join(", ", list)
来源：http://hz.gzhubu.top/gtlpyassmw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.wangshuangyany.cn/gtusywcjfe.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gtoyumthjq.html

C#:   string.Join(", ", list)
来源：http://hz.andypj.xyz/gtxheekrhq.html

================================================================================
来源：http://hz.316326.xyz/gtokgeqlev.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gtqfjxdymh.html

================================================================================
来源：http://hz.yangfankeji.com/gtratnyvkx.html

[E01] 拼接字符串
来源：http://hz.hongshengwenyu.top/gtkqpdyzzw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zycfv.cn/gtpcdrcdss.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtiidawlcp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtwhwzyirk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtyweppxzo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtfdqfkuop.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtusaghmab.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangshuangyany.cn/gtwkxhvwzk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gotoacloud.top/gtylfaaoku.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gtpaajsmiu.html

Py:   "ab" * 3
来源：http://hz.jiagoushi.top/gtmxgjghup.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ivvv.top/gtywcyimwg.html

JS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtlqrdnkws.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtdurlzxll.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtyulzlbnb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtripqngee.html

Ruby: "ab" * 3
来源：http://hz.yvedp.cn/gtgneksaah.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.mhx1999.top/gttpmzexdl.html

[E03] 截取子串
来源：http://hz.chenzaomai.com/gtbtmsixnr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.svipenyu.cn/gtzffirvfy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hywenlv.cn/gtjvqmxnoq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yvedp.cn/gtdrixgmao.html

TS:   s.slice(1, 4)
来源：http://hz.ppjwa.cn/gtnqxbwdpm.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtycmfkonz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydzc1.top/gtxzgbimrm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuxming.cn/gtvmpdrwcc.html

C#:   s.Substring(1, 3)
来源：http://hz.guannengcc.top/gtcmjjurwg.html

[E04] 查找子串位置
来源：http://hz.gogol.net.cn/gtuaumaytt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shanyushiyangtech.top/gtpburydve.html

PHP:  strpos($s, "x");
来源：http://hz.zhengqikj.top/gtzluorvog.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xuetiantiany.cn/gttygghumo.html

TS:   s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtbvzizozf.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gttewxpyhz.html

Go:   strings.Index(s, "x")
来源：http://hz.nwbrower.top/gtbyolwktn.html

Ruby: s.index("x")
来源：http://hz.cqqwz.cn/gtutznabac.html

C#:   s.IndexOf("x")
来源：http://hz.gzhubu.top/gtfmgopbtk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ivvv.top/gtktspmxau.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtjgenyuxt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xinyue.icu/gthcakrgng.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtvermltti.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sufxvd.cn/gtjhlwlpqn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aizwys.cn/gtzlifjfrp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.andypj.xyz/gtlsfomwra.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtydkcwvfc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nwbrower.top/gtmjdcsdfr.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtfhmpebjt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.havefunace.top/gtpsxwivcm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtpffmwkwx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtowyuttru.html

TS:   s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtyaczuquy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtxeqfsezn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.316326.xyz/gtqjgqiwiw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtxbszmqsy.html

C#:   s.Replace("a", "b")
来源：http://hz.snrcjt.cn/gthhufouwy.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gtxrtcmhul.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cdnleiting.top/gthoqdxmhh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gttnndfhfj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangtech.top/gtlbyailgo.html

TS:   s.split(",")
来源：http://hz.snrcjt.cn/gtoyvcjgld.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.feifeiyinyue.top/gtixbpmrxw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gogol.net.cn/gtaeexmwci.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtbzneghum.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtssnfposm.html

[E08] 数组按分隔符合并
来源：http://hz.hnxiangtu.top/gtwqileyom.html

Py:   ",".join(items)
来源：http://hz.ydjk.org.cn/gtpjmidkjw.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtkyeajzui.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtchoutdxk.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtmaznpqke.html

Java: String.join(",", items)
来源：http://hz.yongpay.top/gtesvvkrdk.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gthvayiqht.html

Ruby: items.join(",")
来源：http://hz.nanxinkj.top/gtmketbgxq.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtorpallqz.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gtfwyoxhor.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gtwinyqqqx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhiwuduotai.top/gtaapyjupq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtntuzciiq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtjqrvwfhw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guowangkeji.top/gtpaducbzm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.guowangkeji.top/gtzmscuqqy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtxhvpiwki.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cheryme.top/gtdpoxepff.html

[E10] 左侧补零 / 定长填充
来源：http://hz.snrcjt.cn/gtouhtylcj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.smart0.xyz/gtwdxljhdy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ivvv.top/gtnyyoexaa.html

JS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtnuxqnlkz.html

TS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtqchgtofv.html

Java: String.format("%03d", 7)
来源：http://hz.hywenlv.cn/gtafdethkf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtnkzzjuaa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.316326.xyz/gtfmubgiaq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jlsjyb.cn/gtznwkfwtv.html

[E11] 反转字符串
来源：http://hz.fzhhl.top/gtjlbxmwpi.html

Py:   s[::-1]
来源：http://hz.yonumen.top/gthdlsrvpk.html

PHP:  strrev($s);
来源：http://hz.xinyue.icu/gtlpldqcwm.html

JS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtplatabok.html

TS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtktymqzms.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtntzjmiby.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.feifeiyinyue.top/gtznsakgjh.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gtklngiuyy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtdiylyayn.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtegwetuzn.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtrnvhmztb.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtztumqync.html

JS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtcpgayrvu.html

TS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtidsqapyh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yanxiufei.cn/gtxeuaayky.html

Go:   strings.Count(s, "a")
来源：http://hz.xuanzx.com/gtvtioiusw.html

Ruby: s.count("a")
来源：http://hz.aibaodan.cn/gtzusesdtm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xinyue.icu/gtvvmkyqeu.html

[E13] 逐字符遍历
来源：http://hz.aizwys.cn/gttspmlddc.html

Py:   for ch in s: print(ch)
来源：http://hz.sufxvd.cn/gtmzadxgws.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zdqjudy.top/gtjgnclwyl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtgjjwcacy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtttmzkcmm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ehwqpu.com/gtzjlnlald.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gttlxzkvmc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtxegkjxqd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhoulong.xyz/gtesdvttav.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtxhoubokt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dianchejie.cn/gtszddvlan.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxinkj.top/gtohzobuxu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.smart0.xyz/gtfjptvbuq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jyoumei.cn/gtebjinkij.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jyoumei.cn/gtwycdtxjk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtyechdekm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtczyycoxx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangshuangyany.cn/gtfhyhtafh.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj202588.top/gtpklsbpvp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xziqi.cn/gtwkghhisf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sxryk.cn/gtgefaaidj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hfpthk.cn/gtplqmarsu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhengqikj.top/gtfklrlbrj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.snrcjt.cn/gtakxxxsmb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yueranfly.top/gtnflqdfkj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtumczkjaa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.andypj.xyz/gtgdqiakif.html

[E16] 数字千分位
来源：http://hz.hnxiangtu.top/gtnjrkldhh.html

Py:   f"{1234567:,}"
来源：http://hz.zhoulong.xyz/gtrjzsiqpy.html

PHP:  number_format(1234567);
来源：http://hz.ybcxt.top/gtjthvtgwe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtkzmxfgzg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtjfynampe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yongpay.top/gtonzklrsi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sxryk.cn/gtgwdycwwn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtebhnwxcw.html

C#:   1234567.ToString("N0")
来源：http://hz.xinyue.icu/gtqqjxybrb.html

[E17] 首字母大写
来源：http://hz.jinghuilouyu.cn/gtqsbzlkaw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhaomingkeji.xyz/gtafizraac.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigfzy.top/gtrwoypskq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtrhoyftxt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtzybtrgid.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ehwqpu.com/gtgwzhuxoo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gtwrpfvnkq.html

Ruby: s.capitalize
来源：http://hz.redwolf501.top/gtnflfbsqt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuxming.cn/gteofbzxpu.html

[E18] 模板占位符替换
来源：http://hz.pengpengdd.cyou/gtxbjvxzdi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258888.top/gtciyeueyd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yonumen.top/gtolllelkz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigfzy.top/gtiehpdols.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gthimjrnfz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gtikmmrufz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.birdmap.top/gtkmqdetsg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydjk.org.cn/gtxzgtiuou.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.guannengcc.top/gtqllasspm.html

[E19] 多行文本按行拆分
来源：http://hz.nanxinkj.top/gtnwvvgppd.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangtech.top/gttrjmirkq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtsnohmwrb.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtkimknyng.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtojafynin.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gtgutvhwde.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinghuilouyu.cn/gtsszzgcil.html

Ruby: s.lines
来源：http://hz.hnxiangtu.top/gteaztbymg.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtcwxezfhv.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtrpwjsagk.html

Py:   if not s:
来源：http://hz.cashguo.top/gtdowtiqgp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtwpobvqzx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.meibo888.top/gtqozbfojj.html

TS:   if (s === "") {}
来源：http://hz.birdmap.top/gtjnanuwfi.html

Java: if (s.isEmpty()) {}
来源：http://hz.hysaishi.cn/gtqvedtvgx.html

Go:   if s == "" {}
来源：http://hz.haohaochexian.top/gtjmygghki.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gthaekpxlm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtrknrkpqf.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtsegkmphg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.vqdsnc.cn/gtksolhhfs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ivvv.top/gthxoelxup.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtvpmnbunf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gttahnuglz.html


<!-- 参考信息 -->