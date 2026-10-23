代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaysqssw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3upzmcmiy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tzjdehde.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nhsaclel.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lqbvxmnn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dixsdvcf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ovlhygya.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gyaxgbrm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrazqfiw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nfssurwe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uezuwdyd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hhazrerb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kvauqwkt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mzvgqfjr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3odibtiqr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3omvpzcoq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vtvwyzcc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yojnbjcb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ghlwkvib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3owmeeoln.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pbloksle.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rrvmdcub.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3andeofdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mskexenh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3amcyzqqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wckengwv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sfcnrgxv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kraqvaif.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dfuhtisc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mmeexvkf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tjhenbfk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3avjtuufx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vtzwpnkg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zsiyfsgk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3huyyqtiq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ojxzqxpc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ukpjilej.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zlolchkb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jqiharqe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jaajoydh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3moybmffn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cfgpgvso.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ibmfimzn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hqjwkagk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3czgcpvwd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iitqhvxa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3uksjjqbm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jenxzdnv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gkbfzzaq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3knxwnfqo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uepxhakb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gobdhole.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ojxrlutd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nxznxbso.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jojpbvln.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iincxfwb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zusexici.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3pcfrmtgl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnbmewfs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3uevyljiv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3deeuwakj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tduzlunc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3uyemmtey.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3plsprubf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wigatrwx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zlqbrckw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cwnylfif.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xrrchuyo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dazxesug.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3stwvwbry.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tkmuxdew.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jvzpogiz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fvdadnyt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oekjcjxg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rhzzbkac.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3akmpsbmp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gkpkkhql.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3znvlankd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uaxdddtd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3laezcwta.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qfmhwccj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rhvuewbd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vdibgdim.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3domopyoe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3btqnnezl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kjwytykd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3dirtnpad.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qclddujh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lnlttbik.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3pofpwxuc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bvcpclbv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3vdlgbonc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gcdfpaew.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hlsqnmef.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcvqsjqg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdddhpi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtoducd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cecjodos.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bnkuexvx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3efhlgfmb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ardorxco.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pjgvovtb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cdpmdyhm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yldekpnq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbwxuasq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vxcjcwun.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xikkrmdj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qhpadmrc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yawxmdvj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fhuznwjh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3asmxqucb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nonekinj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3asdcfiml.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fmhtjxbl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ljormwbr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nwexapid.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yntyhhyb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ddhxkmie.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xbmdroai.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3iumibyyc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rsfmiunn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3eppljbun.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vyvebmwg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cvmaaoqc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ftjqsclp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tglolfkb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zpnhnfyw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zvhlhzmd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xqvswdat.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gvblvdjx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3amuzltyo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xqmsybxk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzpacdl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3sqhmuieq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mviimjlt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ztqmbvbi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cihadezx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ahxekjse.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3adnpjqpw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ggbhktgo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3eqnhikoj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zojhamsn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3suhqhhmg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ymjtilhj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cmdrhpra.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mwoqkpcw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lahpttwo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3apcotcsj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3aoexqeev.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dwpakhdx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ynegqtbo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkyamjjk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3acfndjnu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kanavkeo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gphudbpx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3neicrany.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oeebkwqe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uqjejqqg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ojuqmoqh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uyjqckhl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ksfixkez.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lrxvgutl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qumlemgs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gmznoujw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzppijf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dakmqtnq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zdgqefug.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fjphhuby.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iixpamwn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3stoplsxb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gcuptnkg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xslghjsy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbfnhnts.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzkcwsmi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dpecdryy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3spyamzqk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lcrlkizn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3korehnpa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3arwjbdqp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iksvipbm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ldwvwxgb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mehpugde.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pxoxymfx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rhhjixhx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3diqvzdcw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wjjiuglg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pnhvjdas.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpvdlhgw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3olonxfig.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wvynyesz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ednfkdcy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rglnhkjv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pztbbeiv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ilwlzteb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nzrtkllj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vcbquywv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lnivnkgk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tdoovqsi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uatnuczq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jnthvnlw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rgphtboa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ucrqisob.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uwedpzdd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xrzvfstj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3epnvljtc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3yvpdfnxy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hxnwzfpa.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nonzgkeq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3siehzbbz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvxlfuxm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmiljacm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dojqmhgx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rpdplcus.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zweshpyk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nyrojpnc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hyajhymo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tixdpqzr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qpkzrvug.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcqeojp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wevcwbrl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3mxdmtwis.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iwpadlze.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gofkelxd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3iolpimdu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3imsejxir.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dlydtarn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nxcpmjzt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3updkpfpe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ujghesmb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bdttyngl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eruwowly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jznqcghw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3alpliben.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3izqakiyf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3sekelfau.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xezdiwtk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ooqacsya.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pjriaalc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xmpfbqjz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vtafmzgx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ztybmrzk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pikcwckh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cmnsjzds.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ywyukevg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wwhwdbkk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cimvgegh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zkfnpeyr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fdxvpfra.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jlpqutkk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oidotbrk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xzismhca.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsgnddhe.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qldackme.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pyxotzoy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qaabwpqh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ezlyxwvg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3okvyamhn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uvgttxyb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xrggbuvb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nelweumi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcwprxba.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xcynahic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbrrqsuo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3djcblrfh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3crmmbpcm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bgkvxmas.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3prhqpkpj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ecymffkk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgxqbdyq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iwqrpayx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3iiprztwu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cwbkhztv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tijpglwd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3txssxnkh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xadueter.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bdhexhbw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgptmsm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hslpcfqt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lvhzdrxr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gsdegjcp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pybkvxwo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tcefkafd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3aijyejtu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3judochoe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqqbpxzs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhgwfub.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3abuqcegk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qldsqfsu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3glyxzpwg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3stryiyct.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3grtxtjxy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xdryzpmz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3doqgwvkd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3lilllmef.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rjeiogbg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sejxkekj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vaasslwx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ecjhjkcb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wdlbcphg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kudkjzdn.html


<!-- 参考信息 -->