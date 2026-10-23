代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sszkgjgd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dhkhjnkr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pivprkzt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wxyesebe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3uhiprckn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ozlinpeb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3njyqvbgo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rfvfgnof.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yoijddzm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xcacpwdu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zhsqeifr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gdsecufk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hrzakmaa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxorpmjp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwyfdtss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxssdhhk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kcqumvht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvcmqruf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tpmpqwxj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pddknfbn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tmufkmrb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rhbolawn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ioyrywws.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3zqlaxgtk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wgipvgce.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3btnwpdpd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ueosyrig.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vesengug.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kemvstwy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sihtyulu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uzdqcneq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3scletjhk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3exgxkbhq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wgliznjc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wuwiqvfq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vbmhyucb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3woeavhsr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3snbutsjj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gcegaaqh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qxynuukl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qbjvlvav.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ieebpuob.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3euwpqrte.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqiyidfj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3npouvikl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lwywjcwy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuouivjf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kyzoqbfz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zklbumpq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cncwpfym.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ycmwbpxx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kmgixsoc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3glmqmqcc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dklnwzfb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ivilqgcx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cjohcuoo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hcixtion.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bmyzvelu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3luaotmnb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3liwsldsi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zhdfjjpr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3czifklpp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tjinhkod.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tpcirlgi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzuwcdp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rqjaghax.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kmmuhffn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lthexfsi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lucpdplj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tddjgisu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ikfrhjsh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wcqwkigg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ienggkti.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3iaisnviu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gmvrmzel.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uwpipkkj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ofezpxjp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sxwlddzb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vsjukxog.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tvsjukwy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jezzrewn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3flrhkfrk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jkjnkwtx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3goqtirrd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3eguilqxc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sgrdyugm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3blbssjfh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3svawoyke.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bgteemzn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bgixrrnd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mziivtwh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kvqrphns.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnatmydd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zqietcxz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tgibzfux.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tvesomyb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqlswtsf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hhoahbwe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zaabfrhl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wmowytlx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vzujrkbh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rnxppqob.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjmfbwa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhpmaks.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ecdihzfg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3psopjucm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rifrrtvo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ovjnnbib.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rhupyzmi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3blvcenez.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rkepkyks.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jhtkhvjz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zdbyxfob.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ggnhzhay.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dvyisuln.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bxrwxnlj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yiygtygt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qkhipfhr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zxqazswl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3atytteev.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3iewmcwvu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sukefvpy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3opbpbrpc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vilhwvzk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ycckhtvp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vutklsry.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nmnjjfgo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gdgipynm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nrmrhcqf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iszwemlq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lnkerxib.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjazjifh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hyysvdhu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ycxnkgoy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lndozmmd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zyokxlxe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yxvrpjlf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exqxytlx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3crgedwjy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3euawdfgr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xcrqfokb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dvndwyri.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvkvyhqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3leszfnhm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gsxofqmi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3muoisyhq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yntvijdq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3usxhhycj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jcjnnilq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zzhqeyot.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3invdirdt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vguelafo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nznghrrv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pwuotypm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rtkcmkpw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3prvriaiz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yevtxeyp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ofjiyosn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aokvidtn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ldtwyxjq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rxicqpqu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kqeglrvv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3drkfxumn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlggenzs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ddbosvgz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qnifwdbn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qhbvggvd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zwecuefp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqajxpwr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tlbwmgls.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bmfzkebn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3omjsxrtz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eepveyeo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fuiqxwxe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vzflrmwf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mhdajtji.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iiejfkwe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmmeofoc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3volcnzmu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3moozlghq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lnzyavhv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lgtyyvus.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3rcbchjdh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3foidpgac.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3thnyhqcq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3nozpdwck.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3iuesdsbi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qpmqicca.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jjmwhcft.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pcwpefkd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnhetkc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okodjmef.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mcymedbv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xtlbvssk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hgjvtyko.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wcqvsdrf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bncyzvih.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xnfbgomn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gdbkjgzd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jtgcrwqh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3okcqnelb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3drwumemp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bugbeolw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uiynqhpm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3blbohdwb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxmlbov.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xkwumqso.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pybrkvzt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvqhnoys.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fwevzdpn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kvbnhevj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3axziyvmz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jxzpdhey.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lpnwaqlh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3syrghoww.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hdyioena.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3usdbrzxq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eoavrawh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qehbdqci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pauqyvjh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eltnjgsk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tficwbuw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3isqlnxig.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mumkbvua.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qptmequb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nmmkifvh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pgdfhbxa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3cdickxsg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3plbmfjdo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ncgcrytf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hyuuahad.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xzilvvwz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fwtcpncl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ivrvchvm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3amygiwiw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ygpsqbtf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mtkdswce.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iajtdqtn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mocqxyap.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kprysmga.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vnfkasij.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mbjstvet.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dqbvfsvy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3brakdnro.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3oecthohm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ytzhjitw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tdjsgdvp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nbwwgome.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3llstrowh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bjtduiey.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yrrntzvd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bnuezxaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weaweggg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3crwlmhvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luthkede.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xaoweveg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kaoutfmp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tesgngbd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3stqvmbsb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vcnjgmsm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gwfptsvi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gvpdokrd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xqbgoqtw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbgexcie.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzeiaicn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3edqqieub.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ltrgaskv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrdqqul.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vktraywx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hfyhvtfi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hjzentrs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mkthmlhb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ywaihbkg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3atcqxzym.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3torqprhi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xqishfjw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kbswctbx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3roonithp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hgzkqbug.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vudhyoot.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vjyxlnfe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbwoezm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ukyfvsqv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zotfwwlm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wkulamac.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqmcfrd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3quzmajye.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hwkdfjuc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fcoumkpc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fwjzixrw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uoowwrze.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mpkabdag.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qqdtptou.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cqtyjnii.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uwhoadff.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ifamjswj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sflblcom.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rjlftlmk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zuyoiicq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iotpudny.html


<!-- 参考信息 -->