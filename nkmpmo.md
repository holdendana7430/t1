代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tbfvtjxi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2spsiqhyj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2evqwjatz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pevwnbiv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2owxhyoqp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2npvtdtyr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2krheckux.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfvnphde.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mfoicpqf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wmrdbewa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pneokqcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqpulmfy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kkckvuog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqnftzmp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2msiyikyb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gtaqdylz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2beqanzkb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oyxvzjcf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oixchruk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rijnwifo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2oxtiuxur.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gwayrkqc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wyyteuar.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dtlffjqy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qexmeaxn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lprlhdms.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bijfwumi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ymawqoom.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2arczgciw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ozsybewt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rxybdlhl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wsojduko.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ewbiipul.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hqyyfakx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ohjjrcbm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nytgtnzd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hgsuwppw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hoclgvsc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2agkhydoq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kgeehfva.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ufrffbii.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lcfgodth.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zurecqme.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2unnzaxkx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ijgcskpq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kapqetwa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jfnbosaj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqckqpm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uapzfvfe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mzrsfhcl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rlkssnlt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kuyidsts.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yrsgljlh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uccawtre.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nrhagldz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vvhisyjd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2shgeolxm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yhqbvoia.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jotwiivk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yrvbspnr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmhqbfmw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2truqzmvv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rctlaazh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iuxjheyu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uuscehqe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhapvnc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mehkbtci.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2viiqrkca.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tphukkxh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2osgbafaj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zvumltaw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yehjdjqd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yxmlatil.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ogqzeatn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lnhyydhe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tztojljv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iomwqizz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jtyenrcc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnmzemt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxfgecj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tibuauyv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lirzazix.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tdfazrwe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qkkyyxkc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uczyrecw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xblzwivg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zgwibnde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2canfxbad.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2abcvuzrz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lgcqavcx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2khzbesmp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qkrioxjx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hgwhpjgn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nwkytzjn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uqfstuxp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ilfzycsc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jezudkyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nfuqtvrr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gscmtigc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2degwjdub.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2faulvhws.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2aeotivdu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qkqxhizh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zqrzbwkr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uamwgiwz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vjuzaoxu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2aelzcsde.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ftjjllzy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fxryrojm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fyaotmen.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2enmkhsyu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mftgszfc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tmvuoagg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rnpcmyiw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2soydhhfx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nqbxkkqs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lfwwzjmw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qlrjfhuq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rktgswgk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdjxrgaa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbnkmkdu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qmjmgxvk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xcnvjgkx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lqezghfm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jvypwqgs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fgjgcmvz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gfqlaihw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxzusugb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dehythgu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgtqeqdv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ghjlbzol.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2szynneei.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ahkwtncj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gqkuvkie.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kgvbhjpe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmtszeik.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2abiblxqm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2urvgwcsp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cyypqksg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dyuexkcc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wwamhrga.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uszyospq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2znarvghe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wjhjngec.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ljujzbps.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2iofksqlv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mnhokqvw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dhrohavz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cslbqvud.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qkunyzoy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmkvxpgb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvlcbvra.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kysvbcle.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ixlkbgqf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2stzvftiq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tnkigilm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hgimxkdf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qjapkgqz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kotggwnz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmumzrvz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gaddipna.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uyiayuhv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2upzukslb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qapcislk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2srnspnfq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oybldkfv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gpktcsgt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xwexhrbw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ljzzjdpp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xdirvwkf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2knnaciof.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pqtwdhwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2goroskpb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwcxxmzn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xqdywbkx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gxfzoejb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2adnbatxn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzvynmjz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cscdyalh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hcrcxlys.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xscinccq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2aayyenta.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gykzmonv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ipqvyadc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bwkjyutx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gcgddqyy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xrsttkea.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cfhjdmgq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ezfaovwv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2evsapigx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2liznihzq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2surwkvht.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zhncwkac.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mzfvhlus.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yokupxez.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2olvyxqxz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2chajokla.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mclmdgyu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2raxvrsdg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpyovbip.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qaoylezm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gcpxyqbi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpjbggy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jnfsdbrt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvubyyn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dfnvppxn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pulykaaq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lpnpjdsc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ejyngqxk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kogoixyi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rtzgqyef.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sehndahi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hbjzbdju.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zmhurrie.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zgpnzknm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hxcxwwfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pbognulb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2leffmiik.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cvwuzxmb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2aqfopsbp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2biwyofic.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dsgbuvtf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ynilveiq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogsujtnd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhmwosp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wzwcxyhp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ajxnlbpp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mhahpwdx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2izubylpt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2krksjzfq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kposiumr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mnklwalr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sabsycso.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qnzjfrdt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2kdxugorr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfpjviyf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hbhunltv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aeyysomd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsycrznf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xpkonpwm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2myzyipcs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tolbmuwx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bcucozvf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wzwipeio.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dbyqgefu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fynoujkv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lndninxl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yukfkibm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyqalmcw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xsvmljfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oojudjtj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kzstfzwz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wptiabjx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qpcpfndb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nzlawijo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gfnyhylz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygieogpk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jrtdzghe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qtovexie.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xpuniucv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uhlfgsil.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2swxtxell.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qxxwpmsq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rjtdbljr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bzqbfixj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxqukqbz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2glfezvrf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kvnqjhsr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hrqyehlr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oyquepoe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jywqebma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yrlexuzs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nvswrhws.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ugkjpxfm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2julfuhzq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2phdjbply.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ireurzww.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xwrgiacf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2klafuhbe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mvbohvde.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ncamnrvn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jrscqvsv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wmhbefht.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jvthsshi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nogssbez.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2friyercs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kfnyhkdq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vbkwiyzp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xdhzikat.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pqhtkndh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2msuflmmm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dydwwmjc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eldmwemj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qcvetvrr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ombigetb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zjmalclo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2glpdmlxe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gxjuxaff.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ygfvgskk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uqsoyyxd.html


<!-- 参考信息 -->