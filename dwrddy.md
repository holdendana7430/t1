代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ymjjvnhl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzbfqlll.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vkvqrcyk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mkdqdhde.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3sqjdbwap.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vgqlrrsk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3nimqxrzf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sovgdudv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qjvrgfll.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mtlptdcw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3arbuziaz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kccltfqd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3lwobmbga.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpxhhsif.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3apniyqzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djxtqrfb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uxtntxsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmqfnxpj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wdpserao.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ysufpqgm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3piyzwtja.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dqfwvnqy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tpainhxy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cvefhxiw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hrmftcfz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kbvstydg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cdybgiaq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3kqtmhwyq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ojdoxtzk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jdarearv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xzvjvzou.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yozmuzbo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ovmkhcpv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sbajurcv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3oawrfonf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qfwciwbq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fuiyewdb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3myxsuxko.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3oexdkgyw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3wjlhdcio.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3krkzgsph.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ejyevlaj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rcblzrjs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gdajourr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fhanyvza.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vplyltln.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lyxmoedz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zuorpciu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3weblsxyo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqdmlbo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vkzfcqls.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3cyydcduv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xpyftvgp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhqaeait.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3eloowavp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kyylwuvq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yvftfarq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ljldyjny.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tljttits.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3myrstczu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3citohulf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wwgmmrrn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ikbivukr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vbpbrcal.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mxvgyydu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ykfrcfcj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xwxrkvws.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sqhbccgp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3diaahfye.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kcikjudl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3akpuoqso.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qhnzxcue.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lwhsxoaf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3cmrjjsng.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bqoxfzju.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qqonhxaj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qmqknmpm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yyswftpq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mftioxyv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ddhqflus.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kcbuswux.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dptmqwkf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3krwlrfar.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dflnyost.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ghabijiz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3psligxee.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xcwdkqnl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsfwjeu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zpfybtag.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eebnbyil.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dgntiowa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3famzooty.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bpyrybeq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dvwkifen.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vzjcypss.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jicffzkf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dchqsjcu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ozajyhnt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3voensnyd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cbctlykt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3alaonron.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fhdnwgjx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ijobhglu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zdzabshw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3msidarzt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3avkasyfp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hwdtivrj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dlappfku.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nisxobmp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3favsjswl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kshpvdhl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zhccebkc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xtddfgfw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3izzvqmyp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3duzxwuei.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3dnjtldhl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3yigqrnik.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kpgybwoq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fgjzwpda.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3chbiichl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kohiumwb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qnnfqbbg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ngxxprxd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrfmxtgn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yivqxdxx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fiffdtqr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kigoreis.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ddgewlfy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uqrgjsbx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vjvmlibp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpgfmcyb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tjwycajl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ndmpkbgt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zbswhgaj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqkajlfb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3phjbimbr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fcjiwskc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjktugsf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3agrjcvky.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3aswyjfcu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3olebkxjj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3amerpfwl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kjefdruc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bklkuoic.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bphvvlhb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xihpguno.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ubdledkx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nfqfrlot.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gnsdjcsd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nhsrungk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3soeygvba.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3esixdksu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cgrqlgym.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mwfhvbgw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bsgwgnep.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgjommqj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwhhxbj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxbsfndc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mdowroib.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wbemlfvc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kzvumrhj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vnaubulz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jtycxkng.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ymmjfwlw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lmdrrmgn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqqmqjgr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nxvrrjkm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gzpxaxxh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nuadsrnr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zknqwezy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rurthtuz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3irhcgrtq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nhaukbda.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ufdsujxs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcqgwhw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3aejxyecs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bvyyzklh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ndzpceoo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bdsgntjh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tmszwhog.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3znelijum.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pcmdnpbg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pptjguyb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ocpjmiuv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wosxzorf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gbmhoxlm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ctzyfici.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3swtthzhp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rbdyhipw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mujselhw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzqegogb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oyonvdpu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rojchzxo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3plkuuqjd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xtsnurkl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tsnlvcsr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3slqteftn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xupxqmdb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tgtdjzbp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3oworleol.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mzeknzxj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tguqjodm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqyvahqe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atzoskbb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxjqsnw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3btekabvx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hbvseepu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nbadormp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kajkjabu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ufrjmgla.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amlbwnnw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3amdaozhn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tlpcalrm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tiponkbu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kajqluyh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fqgjvajl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lbryigwd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kdtpqjwc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nnejlfiw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ceknzjnt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwvadzi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pvaoombt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qfatijao.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3iwqeuanv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nvoclaxs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qknfpjeu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vrjgebwm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xqdvbnrb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnpgllq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hxcwuuth.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehaiyzcl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3sgnjgbzw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3oiehppvb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tzeirsxb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zwzwkafl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zkhjimar.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bixkpxdx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3spcfrmwb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaqecnyj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ncrwsjuh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fxnuzoqz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zmnmskfa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3feudyvlt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3cjaosvcd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vjzyaeyb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3odxenrbf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3htycagyu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qcdqssmk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3skfnniky.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pssakbpw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fulgqgba.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3moffxwkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkthlwfi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3fzipaocz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apcpcuzl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mzbwtrdq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mmliqmkq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pvpovdhz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fbfosurn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wausfpam.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dmivrluc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cgruqcgh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nuvhurtx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3akjwazfd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dhbnssyc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pacfnywg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xftfffll.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kfvrjtiv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wffgxvsj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vbftawze.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uyowrnof.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sawrfqqq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hcahhvde.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vkydzvxw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sceqeion.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sjhlduwa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uajxvqym.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmquufd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmsggmt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3abhdvnum.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xhmmlced.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdyyugb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hgtcyhln.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eenxxcji.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ksvunlud.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rcqkemkd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ykhsfyan.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3btmansdf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bmzfcfce.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zpmorseu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kyfjmlrp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3abocixhx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xfoqnify.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jwlcwwzm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cewvokek.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zgjbgyvv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3obvfltuv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zvrkrluz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3szzswilv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uxucuzxh.html


<!-- 参考信息 -->