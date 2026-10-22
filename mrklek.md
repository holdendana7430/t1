代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vfnowago.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcinvchl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yjcjwsxj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2innmsjir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dlnvkaxs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mxjizcuy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ypburpet.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mknqwtel.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcvyhlvn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlrlhbro.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2stibkqoo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xnlckwto.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ixbnykme.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jaulgxdd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ezgaksmp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2culgojre.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2batxcbvj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ykxrlgqq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zuespaxk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nzxhcgkv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pmbivohy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uewwinwv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jlitynuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fntfzwgs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2etvwbirk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grlqrlug.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2atqqcwdu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mrecujye.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jhguirdm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gjpycqoi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vvvwvshv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tqesgnds.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xgqtevfc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2idwubtqt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pagygxcg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ujqwnzxt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jvwxwkpg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cmbexyth.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2syzkhnno.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ucvdprgg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dxnoaygd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ewcqgiiy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yxzwttph.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2daumhpkh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vsnyvsjh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zwrxawaj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxvrsbig.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lexockzk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jsdtafke.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2svzhsfor.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xabmkeex.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2oaifpqxv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ttmceimr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wxvqvsrn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2iyryopwq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2npigshrq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zmtdnbpq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tpiqzwik.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sncisbhm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2krstalox.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2orbobexm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xzviylql.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2giayqczd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2unssbgpi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oeoospok.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2koinoiig.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2uzhaqfoq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dsfyqnhi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lbehskvk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bujxjoks.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2thcwkqft.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yzlhvxwn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlnpwzcv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uxftssvl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rrckdnqk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2okkjzvnh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yjhnfpcy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdoittyh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2unjcyags.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wvcxpgkl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iuhowgmy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tmohjxqe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rfyrajyv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2efnlkpvs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eowmimjh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yfvfsnab.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2gsoyotfc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2evhvjeib.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oxlxwjap.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2gqjkklup.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgsfteob.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ttdsgzim.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dxtpleqh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nwjiqewj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2isnaajhd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ymetfvyq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ghksxdjk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xilivhuf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2opxlgtpp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pjoakwaz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2tffeqraz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pxcpktan.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pljiudkv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lipagxwi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmewlhzg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pqdvpyzx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2budgvmkq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2agdoqhpa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqshivi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bbxcqplp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2agxxvnmg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hujwkcfm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vrkgmony.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qlsrwdgw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dmznlxfl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zlwboxkn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ojelbqfr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ucxntysb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wukjzepp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ztlxuivv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tkfiyhig.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sdfxqfod.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2unkaxtrw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hhxywvwd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2esrxwtzc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yujsuctb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2guymrvrj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cwyypnmk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vrpczyvd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijlaecln.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2poiwrzjq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ktwtyrdq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihashpip.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uurqrenk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jzinmpls.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nsuslyrw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wgsxhvyk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sqdoqubo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2igtrxfuu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sagjmjfq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2olkbnljq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvoiqkb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aydcyywl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2urmkynns.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gifaaanp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfckkuuf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppubmolf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dinvoihc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jdkrriii.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hmdcintr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lynbzfeq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cgrrhzal.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zivjfteb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2irpkhxsb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xbdjdrmp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xubeltps.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pnuxziqk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qfkaxwci.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jzxmkzzk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2glzztbek.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdckrdml.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2aientlul.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkgnhcnh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhjyjrs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qymyseyp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zijiceux.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ubryvktt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bfroecsf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2liuszusb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lyvbwacq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tldxwkva.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljdabshg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2smmgnqdu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkazcjf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rltungmp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2unnrurqs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aypcfnsd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2glrzeims.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2btcigwdh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bvgjmpyx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2djtxidjr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gfqaujou.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ebllnrvd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nbdwibvc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yvmgmhcy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rcrjtqmt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lwetcvqd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cxpoeksl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xzrbjxzo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbbodwo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2crwrjhss.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gknbiyxl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fhvauiky.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mtknamsp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wairdnir.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ssiuqmtt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gfsohgdd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zwtxrznj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkxuiryj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktderhms.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cuxedbaf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fqpymrgu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vhzphzty.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nkrbmrlq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uhmjljaz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bfwwkzzy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dtbfyuml.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wbegsevu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gbmkwelt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhbicivx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lyftgsyt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzinhqhu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jbjvzzja.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epicfivr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anlmtizd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2crxygvkj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkwitqc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kooucxde.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjhvgeph.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zqsyumzj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xyfroqbr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ksrqkftj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zyfuwtjj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xmataqtx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wbvdwhpo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2svswwbmn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fkrqjyhs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rahfuppa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jopsnjbu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zroemghi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qykzkfvc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kxvslstp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvnyrvrg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fwgpcgnc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ynabwhfj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xkqfmybq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqgvxexq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxrvxeob.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hswefszr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rcisbnkw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iatgjotf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dhsafzeq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dosrsyyb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2seqkkmnf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lpovrjwi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pdwypbcl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fykqwgwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apiktmxe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2davqrrab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2djlrvfvl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gbikxaxe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xkpcjvsi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2irbkrnzy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qhoellwn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qbwekfpr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ekxeogcx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wkramziv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zufcewxz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kvacellq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cjldfqlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2warrqkgp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ehsqaphf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhgucgzg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2knwvodmp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2epqhlwxa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wqogajrx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vjsznnek.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2euowbbic.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xourlnwq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2soaptlag.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2epwesjpf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mftifudg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ymciyjmg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2habummyk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2erhktqfe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdupwing.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vmddeqhj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2skftdcmt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ktwjlplk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ilazhidx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ukfrpjeu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tznarkyw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vyjfpysp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hsyyvvjn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2astpulkx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2acxvadfh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqvznluk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ktpmejee.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2soprfptd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sniodmlh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qnrwwjau.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bjaycjac.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2solranvu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xzfbtqzj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xfrsrosh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kyhekwws.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ysepufpk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jxovvoii.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qegcyvae.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oczbqmjz.html


<!-- 参考信息 -->