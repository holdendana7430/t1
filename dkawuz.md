代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3raggbslt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3arwaorbq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sznemedf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vvpgihto.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3oevxnlrk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ljycwzwb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3khwmnupq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xqwrarlw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3epenwdsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qvmxdbgg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3etbmwkwu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ogxlkqag.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mmaslccd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ecvhxamq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yvajhtag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpqkhldw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3afioxkaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcehveep.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3umghsorl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eexjlaej.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3drstkiis.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pcihplhm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uyvzhbkl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3entzcegt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qknpdcqt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wduqtxhb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3skbnzktl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lvnzkilf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hcejzwnu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3peweuiuf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dwtjdteb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3polfytbh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dwwxukae.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hhcdugfx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vqurqttg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rwxqwgsz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wvydkzhg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ehmhbmlm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mcrtznrj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3aarjecdd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cafzvqnt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rwmdjbca.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ndbhzcin.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3btsnhszg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fueigdan.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dxnjpdjt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xnsvoxwj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nadniybm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ssudtsop.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3shgndiyj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rjjlavsi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3sqrhvozt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bikoczma.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3phjvmubj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3veokqcqd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kleulwdx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ltctyikm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mwlnwciu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mhftfnyp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cuyuzjpu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rckymkgu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tooqsryw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dlefanxp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xbwbvhpi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hpnjdzuq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dvtwveay.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sakvmene.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rvyjknjc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qymoexmb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tiemihwl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kinlnyzx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hltvfgov.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3sbhysetj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hedwwqgl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gcqpvjrl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mlrxbdtq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mannslxk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhgztfj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hhscjrhm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dbxnlptj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dmomvuof.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lnbialan.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3klzzyusy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3owrwicrg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wlkfcqvq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jalqwtjf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3oykzedsb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3crwehgmy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pwffyrcg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oozikcrr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3aqbuzrgo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mkcemmyf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ezpxakhi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hgvtppab.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ehgktynt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3iyxxukcm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzxhsdo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ptfuuzxj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3svzycoaw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sxlbxwsg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3owktscrr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kfyqjrhw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzonmcv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ndelrudi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zzlaebwp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3amepukoy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qdsvqcmx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ebaieyju.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ewxwlyme.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bfxlgcof.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jrkpijnn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3nadvvjuz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ffjzbqrs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cmtrhvbw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxwlykjv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bufhosnv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hsxwzbsd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gxhrhlew.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3akxzryde.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xwjzudnr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mehwfkmc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3llatmxyy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kuloekjd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3psbsynqa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fegyygjn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3lopyuibz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3shoikftz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pjyjkwyy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fimtywjs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dhtkvaul.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cmdszght.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjvwwfzn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qjmapcgs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wgpleaun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ifiufkdo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3eyfvywap.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3sbgfesbl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zruufilz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtryjchv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ovywecvb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdjyrrto.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3buuwluvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bmgiiwwk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vpulfvmo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jwmynptv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3napvgeua.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3elbwxixw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3udbyurxi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3akohjdme.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xqhoazlt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nywcyeld.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iejrzkgq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ntbalpae.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ambskgqr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pnglsnjr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ybcafhig.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbveffha.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cobjafvf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3uqyslzqj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3smrupodl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nrmizzra.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3elcpshwm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tjbrhmuy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3puydncza.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lpqfuxcm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qdffvjyt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bdhecelq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3icgrswmq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmwsntcf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3liovwqks.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xsaawsql.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3scvjmtvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rssltxie.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3agcknozd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3arafanac.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wypjhlfv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bcynfesv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ebkpvrau.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lwrwjshk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ekyjnelk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3dtxiatny.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3apzjigyl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uctsfadm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xvpcjkny.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bhmpsfmo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lcgdzcus.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3pkmblypg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvcwtyu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3encwkcia.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gypwkocc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pifsbdwr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xsnbkrpw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dgufrxyd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vqtzmlwb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3sogyhdvj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zzemwcup.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vmszynld.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qcpojddk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wqodmbyf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3miwhvkaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tspjapge.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3prfhacxo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jepaqapm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecfeiepn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lforwhze.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dlppepfw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mqzyzhnj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3omlcbvgm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmccujro.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pmedciir.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwombij.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rdgktbpm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3krxtnrxi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3enjouywr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gqdrszmz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jyzsijlr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3iauoptku.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hcsoyrqz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ubwfeebi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuwgxmx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3enyyfglj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xgagrrjp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vgobjlkp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3asjktpod.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzujfrmk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wmrsocdm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3azrgztqr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zdaysdji.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxtxovs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ndtydjho.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tkgcnghu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jdgviiaz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xxergdqn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3inkmukvc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3olaonsnz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tlquwwaf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eosavaxy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wqvabjxg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dhphhlmu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eheejsxb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wdqkuaaq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvaujsr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qmgmncrf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rjildsdm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wsuvrctf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fbsabqfb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tpniupyg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xrbkwvth.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eiszynfj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3udeppnro.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hiadsxyy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xyitraxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnvsvydu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dcqmpbow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntggrhug.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjimtrvs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3njowbfqx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cwmlkndm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3duxiuase.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3henikeut.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vzccpnjf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3opyohukv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3aykjptlc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jfwsedad.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mpepvxic.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xqrwtnwm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3koiuucms.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwtwfmx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vuzrvlzt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hqlqhywl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wsijbqei.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vhlhjtns.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lioxcubx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rfnqhiqv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3whhivrtp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hccvrqqm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dffqtndv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pgtquvxx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3olkcaqhb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pxfujpku.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rytphgiq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bkcpdftu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nvgpwxwz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uvuvfgom.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3aeqktoam.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qepgepix.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xfknwrad.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hyukptdd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3efwbxref.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jratgyhu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iugfvlnd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ddtvxcgc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fvblnewg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tjlaxkbb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ltgqckmx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lsarfiew.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lbnbysfa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qsjzgkyh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xnqkifll.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hnielwbh.html


<!-- 参考信息 -->