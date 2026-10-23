代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cdeqbpff.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dlcmuhtl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3opitkanf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jovbkvkg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kccwwdrc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3crfmnrwf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlajjicr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkgavqan.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3focxzlql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oduavqgm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dlktqemg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lwriliks.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bslzngoi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sljhfvae.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mhufjzyv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yfyyisfn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cgrufmqe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vmfuszkx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xzqvfqgr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vdobbyne.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3eihlzyhn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bvfpgbbx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nriirvih.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3iclmbsgt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3igxqoeqq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ubzwvejh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uyjhloxz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qykinglh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tilydqbj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wrndiwys.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwhydbnh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cfkjqsny.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dapmvyvy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ukcdcbxi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nasixhbu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xswovodr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bomxonqf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qjkuxexj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwhnhajm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ahmzoait.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3evaxdefs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3smitsicw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nupqjowz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3dbwbgxge.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ehopzccr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ymevioae.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zqmopobh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ysqgfuwq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yyrtrcur.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pfiwjrxy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fopziuab.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3byfcwcyl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vljscxum.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jmidlsxt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mvzcwmls.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3muvylnzv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3djvrsizo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3naotyium.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ximtovrh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3icvxpnhq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3tcymafyb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3moryuxzd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vagwonaf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3davswtzv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3clrxmcke.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xzmurlbx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cziufula.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fylrwgrk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3msizrdwr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vvzarujf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ooomwbea.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3goruxhgo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3usziydjm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xfkqkvjd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lndvlpub.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ebmbfkfq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bjwyxviu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vyzkmqqk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hshgujnw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dmpnjmsi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jexfeonb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nyogimfk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jbrkvalg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gsizyzoj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vbhlydlg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3icwlukom.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3osimpzbe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3thbkhyxq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcpqlqxi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zxavgdwb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ihuuwkso.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3oynaelwu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oabruxcp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pqkvsqdd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gkikqqbz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bjlkozxg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zdgltsry.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3idipwpvh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3phazvvbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3wfotsueu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pkamnajv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nqffyvri.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xjdgrdtp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cawluiqx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wpalnxsc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3knbhaovm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rizctvfs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wlpsjkim.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vpzxsmpa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mtlgsqez.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ejegkowx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qubxwjnl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tmajxgdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hynekpth.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zypfymsv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvcsdqg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ywftjftr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vbdwvycn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wbwislyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3thwbbwbc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dahkaglh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cvfjhzim.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yjvihdlj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mgvwtoll.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3oluobchh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywnfwxkz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkgazefx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mevoubqo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3iyodktjq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pkjduiyx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mlkxienq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gktthqli.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfkjnznw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgyhiexa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rzclcqpw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rugifwag.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3drtefmul.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rqufsbqo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhpqmyfd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tnfizrzt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fmarixyf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sftqjiaf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rpgzwnje.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nbtddrty.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gksjdtrl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3brceeiyf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjbaydis.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tqogxmtg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlejatxj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ebiypeqn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zopramvs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rrgudazg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3avwxmmlp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sengoxsp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gnhcsxnh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uacvczqw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dpqequxf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3arfmzxqv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbygpdpt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3urpgpypn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wpobicqr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gkfpqzwo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fscolnxl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ojdgqvyi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3oddwtpav.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kfrrytaz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3erbmrvry.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mvowowym.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bbzksaws.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3pbdllpmp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3einnsfhr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pfbceebv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tjtqikcy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rakosbik.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3aplqubzt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wifggnsw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uxiwtynn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dhrdvbbh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cbqjpeqo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3cvzbucyh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3srcrdlqk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zramsvle.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpyxhnlf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwmcilsw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bizvtqpd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3frvbxmom.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xxdzazaz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3albzpvcs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pszqanqy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gxandqlm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bkqbfmgf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3widznhqt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uzhqdwgj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gdabfwkg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bdvtnntb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxpfqink.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bfsjiqep.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fkgwzgzs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3obmywrdr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3yhdlgtsu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmfzrhj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nveimrnm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhzsvbf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nehvsbgu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hmpqujwl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jqjwdmmm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yeajxbcj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ykkwslaw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dorxrblj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jwdfohfj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uvkopudh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bmyofjrq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmrlfimk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dykozphc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cmqydfuk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zlqzkuia.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3utudlqhw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pwzwnaaj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bzzaxfrm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gigxzulo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ledvvsyd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lehhnezi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qoowqooe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gnonamwj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rkvnzjpd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uvcfcjxs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uxyldmxd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fqcsvscd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ccztgdzb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dmtxzhxw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gxhdnoim.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfntmayc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kbqiwnem.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3yopkhvnn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wrdubncd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lybdhuua.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kxlqyrgc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ovnqnbfr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xogbzhbj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ycsvlsrl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mbclinqv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xocagyhs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mxsbzwmo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3scuadvro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdqfyerk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nxbmzaqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kascqdsf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jnugumct.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3upikxvaa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hhcigkgk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dlldjebw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zgwfbbtt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vawodswp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3dndgebxg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zafkfkrb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cpelbula.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mqvyhqsv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ashhqcub.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ffaqvmop.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3skdinkbz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eqknoror.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zhptglza.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qddrudho.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jmnsvsey.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3htggisas.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cnupnygk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xnwygicy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vehhdkwx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbfhnujj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ztxeynxz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gmbnpvjv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sbmpfvrf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ipcupxsh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzuzrrh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3meqdminx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tdtmfnrd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wpweymtu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rseecdjr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vuzwkbtu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kzxohdqv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wfwtbilj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hjpebccz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vsatntpe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dvdwyzty.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wbxbxdov.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3aqtsopip.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3adzbzvdi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kjohbkdn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tfhoqxpu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mvdiddmd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tfsepdwi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fpiiuind.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ytzoduxn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohnoauuh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sozppvfi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hdjaoayl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xasagfgj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hisvyukt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uphzfnrv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lumtnmms.html


<!-- 参考信息 -->