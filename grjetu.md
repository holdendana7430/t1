代发 wailian999

[D19] 按字段分组
来源：http://hz.jinyuanbaomall.cn/gtipdemojh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtfxxmtwwt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.kuanghao11.cn/gtniprwbgw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ywan-chungtsiang.top/gtpyfwfeal.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.0kj1m.cn/gtjxewuizt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guannengcc.top/gtfwrmjusp.html

Go:   // 手写 map[string][]T
来源：http://hz.yueranfly.top/gtcjnoakcq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xziqi.cn/gtowifmkam.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gtnwqiyovi.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtchvbzeom.html

Py:   Counter(arr)
来源：http://hz.ivvv.top/gtsalrsdam.html

PHP:  array_count_values($arr);
来源：http://hz.316326.xyz/gtmxtpilxz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtujbjkboi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtgjmrdxzd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aibaodan.cn/gtoowpnkip.html

Go:   // 手写 map[T]int
来源：http://hz.xuetiantiany.cn/gtbcfurled.html

Ruby: arr.tally
来源：http://hz.shanyushiyangkeji.top/gtmtijwoqi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xylfe.cn/gtnkpvyrto.html

[D21] 判断是否包含某元素
来源：http://hz.havefunace.top/gtampuiyov.html

Py:   x in arr
来源：http://hz.haohaochexian.top/gtstodcyqb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yanxiufei.cn/gthwjktwvh.html

JS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtoqlbvcfm.html

TS:   arr.includes(x)
来源：http://hz.yuanzhike.top/gtaonkuegi.html

Java: list.contains(x)
来源：http://hz.cucudq.cn/gtxlfffvdr.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtqxuextgf.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangtech.top/gtgtsqwpxt.html

C#:   list.Contains(x)
来源：http://hz.0kj1m.cn/gtmihaifyf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtfemklxyi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtvvgvsryp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zdqjudy.top/gtytkxfmgg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnxiangtu.top/gtvrvsjnik.html

TS:   [...arr];
来源：http://hz.snrcjt.cn/gtcitdniqq.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtuqngtvgs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jianghu66.top/gtuytinrft.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sxryk.cn/gtkrowrhcy.html

C#:   new List<int>(list);
来源：http://hz.zdqjudy.top/gtrdllmuei.html

[D23] reduce 累积计算
来源：http://hz.yonumen.top/gthwktxopq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xziqi.cn/gtwoctalwz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxinkj.top/gttjufrfss.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtopelrwxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.bjfxy.top/gtfxzfthwq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gtkjrzissj.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtqimqqypn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtpchnuyng.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cdnleiting.top/gtaxrdhekb.html

[D24] 字典 / Map 基本操作
来源：http://hz.havefunace.top/gtrlzhbdth.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtkmgdonie.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnxiangtu.top/gtexdpqkdx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fengsongda.top/gtdvrqgrjb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.guowangkeji.top/gtjuqbshjp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangtech.top/gtprqsidep.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gteyllgskx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ppjwa.cn/gtdgxxgpmh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daxiang520.top/gtfqyktqbl.html

[D25] Set 集合去重与交并差
来源：http://hz.aibaodan.cn/gtofpgmcen.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydzc1.top/gtocpkfyyj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gtotqzudyh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtfnrdipmz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangkeji.top/gtkudduhor.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.9152youxi.cn/gtqjznjrmn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cucudq.cn/gtcsslsxvu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gttnohaxzt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gtnyghmtdh.html

[D26] 数组转字符串
来源：http://hz.daria6918.cn/gtoywifkul.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sufxvd.cn/gtynylzuge.html

PHP:  implode(", ", $arr);
来源：http://hz.havefunace.top/gtcrjrughq.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtcenlmibr.html

TS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtbusnktun.html

Java: String.join(", ", list)
来源：http://hz.jqgufenzy.top/gtuiurusvc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnxiangtu.top/gtddwhknhb.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtyhoodcdv.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtfelbjmzd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxkceltzt.html

E. 字符串处理
来源：http://hz.pycfn.com/gtllgbbxyj.html

================================================================================
来源：http://hz.yangfankeji.com/gtqonsvyyu.html

[E01] 拼接字符串
来源：http://hz.svipenyu.cn/gtbjwvmbtd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtixpsjnzk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cucudq.cn/gtmcsupscd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtdszhfajj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtiyzilckt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gtybgeayay.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pengpengdd.cyou/gtjthqxwtw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shuidangran.top/gtkqrjhlnq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jqgufenzy.top/gtsdfkwdoa.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gtxcgyuqos.html

Py:   "ab" * 3
来源：http://hz.yonumen.top/gtqkwhovap.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hfpthk.cn/gtulmshfga.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtakyqktff.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtgunzbagb.html

Java: "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtezeconwe.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgufenzy.top/gtmrgtspcj.html

Ruby: "ab" * 3
来源：http://hz.yonumen.top/gtbjysxgsn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xinyue.icu/gtpsdwplql.html

[E03] 截取子串
来源：http://hz.tian-w.cn/gtjdzxrvjg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtellqlcgp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daxiang520.top/gtmipkbzxl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.52xcode.cn/gtlmoxabpl.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtiedemkcx.html

Java: s.substring(1, 4)
来源：http://hz.cheryme.top/gtjxfwfjsk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gtylhwqnoa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tianlin.xyz/gtsevaeudc.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gtelwhhozf.html

[E04] 查找子串位置
来源：http://hz.havefunace.top/gtrqwihygy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj20258888.top/gtxxkltfnc.html

PHP:  strpos($s, "x");
来源：http://hz.cdnleiting.top/gtckyzlyhq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtjuvbugqj.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtaeuycpor.html

Java: s.indexOf("x")
来源：http://hz.chenlongwang.top/gtmszbjlxa.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtfoarfcuj.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gthwopslpx.html

C#:   s.IndexOf("x")
来源：http://hz.sufxvd.cn/gtqtziojkn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258.top/gthtvtphji.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shzxlz.cn/gtvcclacjz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hysaishi.cn/gtorpmoedz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gteqrqwnru.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.daria6918.cn/gtumrixyvl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gtllvetimz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ppjwa.cn/gtrzpxfogj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yangfankeji.com/gtqplwxqrf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtwdbjoewc.html

[E06] 替换子串
来源：http://hz.hnxiangtu.top/gtnuhhzhcc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gthgcmnlsi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.havefunace.top/gteqplmwzp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtnhgiqbkp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtzbvclzcu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gthivgovgg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daxiang520.top/gtqyxdscfj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtuoamyaib.html

C#:   s.Replace("a", "b")
来源：http://hz.birdmap.top/gtmyqigrma.html

[E07] 按分隔符拆分
来源：http://hz.guowangkeji.top/gtuytjepar.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtbvrvebix.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cashguo.top/gtgscftvac.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangtech.top/gtvxosuqbh.html

TS:   s.split(",")
来源：http://hz.xingfuxueyuan.xyz/gtqhdofojh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuanzx.com/gtmqphuqdt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtuagasace.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtrsgznxgo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258888.top/gtbhxrzpmt.html

[E08] 数组按分隔符合并
来源：http://hz.jyoumei.cn/gtvblmczzo.html

Py:   ",".join(items)
来源：http://hz.jinqigufen.top/gtimeokfkr.html

PHP:  implode(",", $items);
来源：http://hz.zhijiandao.cn/gtpfofhzaq.html

JS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtuqobfjsz.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtztcdbfkg.html

Java: String.join(",", items)
来源：http://hz.jianghu66.top/gtdjtdsbrj.html

Go:   strings.Join(items, ",")
来源：http://hz.xinyue.icu/gtbecpibry.html

Ruby: items.join(",")
来源：http://hz.kuanghao11.cn/gtcmxychfl.html

C#:   string.Join(",", items)
来源：http://hz.jinghuilouyu.cn/gtbwjywrde.html

[E09] 去除所有空白字符
来源：http://hz.redwolf501.top/gtthxsbykl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtwwipdzal.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtiojqhqor.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtnthaqose.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtyuohgmyq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daxiang520.top/gtilhjpsty.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gtupkaqepk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gtyqrtxkns.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gtohmcvhas.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hammf.cn/gtoavpsawf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jqgufenzy.top/gtknugisfe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtmvgmlnps.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gthkxmbeom.html

TS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtuunryqls.html

Java: String.format("%03d", 7)
来源：http://hz.ehwqpu.com/gtmnmcieki.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.andypj.xyz/gtpmuiyyvn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.wangdashe.top/gtqabbqbvn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj202588.top/gtydqxvqbk.html

[E11] 反转字符串
来源：http://hz.chenlongwang.top/gtxsoyqdht.html

Py:   s[::-1]
来源：http://hz.yanxiufei.cn/gtkybgvpwc.html

PHP:  strrev($s);
来源：http://hz.jlsjyb.cn/gttwwfhddf.html

JS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtepjgbbte.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtpyvjcwus.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gtixhjsdcq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ywan-chungtsiang.top/gtpbppcnms.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtiwhmvilz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtcmssrxxb.html

[E12] 统计某字符出现次数
来源：http://hz.gogol.net.cn/gtqqatbxlm.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtnglvbtyn.html

PHP:  substr_count($s, "a");
来源：http://hz.fzhhl.top/gtjqswacpo.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gthezsbjbj.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gteysmthyr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xziqi.cn/gtnfjdinbt.html

Go:   strings.Count(s, "a")
来源：http://hz.daria6918.cn/gtlaofmgwn.html

Ruby: s.count("a")
来源：http://hz.dashuyun.cn/gtvvxlskch.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gtuuxbfbdm.html

[E13] 逐字符遍历
来源：http://hz.jiagoushi.top/gtgyvxpawn.html

Py:   for ch in s: print(ch)
来源：http://hz.sxryk.cn/gtqbfkkjwd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258888.top/gtvdxlkfcz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtfpyopwbs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtbuhuyisp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtygamdqgb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtassrfhbg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yueranfly.top/gtpgpakudl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtgbhkwodb.html

[E14] URL 编码与 Base64
来源：http://hz.yj202588.top/gteufsuqhd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtjpwyogle.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gtblgpyrwt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sufxvd.cn/gtrcbrguup.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.316326.xyz/gtxxgxyidp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jyoumei.cn/gtwcmtkuks.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.andypj.xyz/gtcjfweiqt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sxryk.cn/gthyndjsfh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gthrkjmppr.html

[E15] HTML 转义 / 反转义
来源：http://hz.fzhhl.top/gtidbbzbgu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tanke756.top/gtcfwpdfqm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtiwoforhm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenlongwang.top/gtyojhzpoc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daria6918.cn/gtpcjkxvwc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xinyue.icu/gtyeswjdsh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cqqwz.cn/gtanwuwgmc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sxryk.cn/gtdgkojvhl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtrxherwig.html

[E16] 数字千分位
来源：http://hz.ywan-chungtsiang.top/gtqvvtjrlw.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtydqjiesm.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtgxowyvdx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtpwvvlooi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xziqi.cn/gtowagaqey.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gtofzugviy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.meibo888.top/gtdsxynrxo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shzxlz.cn/gttqdmdtxd.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gtcpctyipq.html

[E17] 首字母大写
来源：http://hz.sxryk.cn/gtrzhronyq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhongyouzk.top/gtmuuzqoia.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.fzhhl.top/gtfzkltlkq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtkaftefci.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtgdjjnpna.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhixingplan.top/gtlogmngzh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtzedalumv.html

Ruby: s.capitalize
来源：http://hz.gzhubu.top/gtcjoeaxlv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuanzx.com/gtqhqvazcw.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtvwxronac.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtbelzvkzg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtwocmjkpx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gtmkjbbluh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtvorvlklf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuxming.cn/gtwbhlkabh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.smart0.xyz/gtksowocwz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gttwvgkgoq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtonelxjkj.html

[E19] 多行文本按行拆分
来源：http://hz.hammf.cn/gttsafdyim.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtoysfxbfa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnxiangtu.top/gtahfbsaja.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtdqlntuwh.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gthiszlmpm.html

Java: s.lines().toList()
来源：http://hz.yj202588.top/gtnywcljdx.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtgxuwocnf.html

Ruby: s.lines
来源：http://hz.jinghuilouyu.cn/gtmdpkromk.html

C#:   s.Split('\n')
来源：http://hz.zhaomingkeji.xyz/gthzhgfwgq.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtafaegzuy.html

Py:   if not s:
来源：http://hz.hongshengwenyu.top/gtejaownyg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnqzz.top/gtauqlyaja.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shuidangran.top/gtixtzjsrp.html

TS:   if (s === "") {}
来源：http://hz.kuanghao11.cn/gthizaphwe.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtoeenhdjk.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gtvetonlkx.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gtampjifoc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ivvv.top/gtcggzpqdu.html

[E21] 超长截断加省略号
来源：http://hz.hammf.cn/gtpewmpaqx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtuswzzwae.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.meibo888.top/gtwrzbpeak.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtojhzhrco.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtutwntlof.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtazsjplpk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gttbzkwfis.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.c1oappe.top/gtvkndprbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtxcswrvvo.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtbuugmnhj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gtzmalpjsc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jiagoushi.top/gthujgsjvd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258888.top/gtiuaglkho.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtvscmuxtn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtguyjudqz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtywruhwda.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtwpehoxbg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtfprrezjw.html

================================================================================
来源：http://hz.cashguo.top/gtupzyjvlb.html

F. 文件与目录
来源：http://hz.haohaochexian.top/gtxdhikqce.html

================================================================================
来源：http://hz.yongpay.top/gtjnuouffg.html

[F01] 读取整个文件
来源：http://hz.guowangkeji.top/gtdjxowphw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtfyfhcqkv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigufen.top/gtzbactsou.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtearcxznt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guannengcc.top/gtriuqlqve.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtxtbgqgya.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtoyyfuoax.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gtuzuauxvj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cheryme.top/gtduqwthpo.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gtqtmjglnm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258.top/gtrqzffjgn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.52xcode.cn/gtrzmymdkh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtuldwpudj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gtwtpbhbje.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtqmrkmtgv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xylfe.cn/gtaynjxptd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtoweigrbd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yanxiufei.cn/gtenihtndg.html

[F03] 写入文件（覆盖）
来源：http://hz.birdmap.top/gtznhccykk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jianghu66.top/gtmmdqdoji.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtcqvkdhzm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtpiratqhw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtrvhcncxz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuetiantiany.cn/gtuuxxrojt.html


<!-- 参考信息 -->