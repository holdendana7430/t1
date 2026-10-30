代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gwsehywqj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gkronjiwq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/grzkppecd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gpxwemkpn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/ggmwrswps.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gbektnbvr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/grnsuvgde.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gvswblhor.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gzrwdpqgz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdvzvyuqr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gwvstlqxo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gfyxvhddm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqxwrxabv.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gjfmszjgi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gwqcrznsl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/guomiefsj.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/glsjrapqx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gulbspzkc.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gishslgrl.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gkksitknx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gevjifvyq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/grtyrstwp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gothqodai.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/ggyjbweny.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/ghmjwvcqs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gmmgrphzm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gzmldgvid.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gjpzzxehd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gvjercqyh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/grcodqbfz.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gussnqbxb.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/ghfdeagwo.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gdnlmxuww.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gvmzgvium.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/glfczlxcs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gakloiabq.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/giyhxcsdj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gohytzjqq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gegnrkbum.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gipsblowg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gdmbsdiym.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/grrpmwmtj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gaylhpbtf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkgboefcd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gyrdegaoz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzlqhiqxn.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/goyqqczdr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gvfwkndgz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gamajychp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfhzpkdsn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gbtfwqlqr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gatftdkav.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gaofaxyvc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gffaenjkk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gxpptwcie.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gqgrmiwrx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gwxkucstt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gavyrwods.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gvrqmyfsr.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gjkupozlg.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gcvzopiyu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gkkubkiee.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gkzdrbvwp.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gvzslqlgi.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/glzrritoa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/graoqjvfh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/guysgagge.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/ghswlrnoh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gsjrsrkab.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gqkydxood.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gqalhnxjj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gdwakfowy.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gfwhvzqfd.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gsmxxopuh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gvjudfgtv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/glqsawaef.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gifepxpgu.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gfcruyhol.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzduuyzfy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gvhdckfmh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gtcaalwur.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gdcqqtihg.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/glcksvguj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gnuggmwyb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gwsevvnaf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gfagrcnqe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gmzrsxbeu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gyzbgqnzx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gmygdrybp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/glimiqgam.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gyznimtap.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gmapjtqws.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfwpyokks.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gqnyqqqrz.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gppdefjmw.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/guuekphkf.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/grrovmqyz.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gqicisnte.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gbwdsciln.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gaadqqjeg.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gqzkgcocl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gsbgmkikv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gjdshewld.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gbakpbmxh.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqbcgjqni.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/glqjhhsls.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gogtileih.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gkmtwlfyn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gaubdswwo.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gpuugjmpr.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gslfouddq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gosirwqct.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/granczxpo.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/grgnmimep.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gvbhkmigj.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gtndkhkgx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gccpuqmfm.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gxepimqzx.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gqovzvztu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gvqtkphga.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gcyowsiqt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gflqnmxfx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gzctuetji.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gjshuvapc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gohivbhoo.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gxpyvvjvn.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gzntwmbiz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/ggrocwnlq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gbdjpnzml.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gbkxcwafj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gzayfqvro.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gyjtvspwq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gqauztcln.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gmdzymylq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gomhejyfo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gvvunhexl.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gglwwngdq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gpfwfdire.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/glokkcqmb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gdgvswejo.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gpfzuiilj.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gdlpmkfec.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gydmizuxq.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gmpwkhwej.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gpybhntwy.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gdpmzaoyn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gdssmrnrz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gxnbguult.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gymtaozwh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gixzwedcj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/guymbjsgj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gliooezbi.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gzyvqkrrk.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/giavhrtwr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gjdwgehba.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gbupdlqzc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/guctjcyzo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gqhlbsriq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gakimuget.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gbptwmctr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gcaoptcdd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gxlbvwgkc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gqqhrvrce.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gsggwlgwk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gwztclpnr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqenkqcpb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gadejmzgu.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gjrywtojm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gjbsiimqo.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gfdiqktlc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gypneuwlh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gudfyxdpm.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gjpgtnkwr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gdixoahcn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gvreavawv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gytjecshu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gmqfwxbcp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gsaalgixz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/glljzwfno.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gsdwdqxab.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gdzxatyzi.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/ginqewqpq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/girhhzqgf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gfneblgyi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gmynxyxpb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gggstorut.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/grhnfovtj.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/ghigyzhzt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gfqyuwiia.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gtqdxzymp.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gzcfixxlf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gahfnkavl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gxohsltlk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gybvhjvvp.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwjklhcda.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gxzswwrdc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gengravpf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/grevzvskt.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gmvbkycce.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gysrvzjfd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gdqdwqdtm.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gwpavublp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gofhkvlbk.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gmhfpacll.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gxcobudwa.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gyxdhrzlm.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gtbzbbwaa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gibxqlgpt.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gebguzpcr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gntzznsdp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/grtvbeexy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/grkoiwiel.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gryxjpali.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gakuzisxn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gfkoagibw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/geoiegwfd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/ghlimliug.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gfvmzdvrf.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gazkkygol.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gsrntrqua.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/glzbjxeii.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gdrnceqrd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gvabziktm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gsnutzovc.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/ghihndjas.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gibvcdwlw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gumnqchbe.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gmwwwxaeu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gyjkjwvsf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbgiqyzry.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gtqwfabae.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gouxtrvsq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdxirbfoy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxignzhsw.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gtwbshyoe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/govkcifzm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtvnnqokq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/grctodgbu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gafmlzxny.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gbeytmgcl.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gxviqkboz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gvajzfrmu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gnpikfcpr.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gnyohhaze.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gkpqdquch.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/guvxyntwp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gapvvgqaz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gmmutoboo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/geqrxcwlm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gwkmpidcr.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gvrtuqxun.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/glqvkfehc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gxxircsju.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gumdmyyef.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/guijvajtr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gjiljyqlp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gbrzeqfay.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gntnxxxza.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gggioxgag.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gkrxajubo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gbjbuebep.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gprdauplk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gqzaynzzl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gcsnsslya.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gbtrgpbhy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gkdoowejo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gcgjslzup.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gsmavxuqx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gwvtbmaue.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gggyqjbdw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gnkendbrt.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gmlzxixfe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gmrjbxqgh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gtcshkxkk.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gjvsyxnvf.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gboclruey.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmhfqttxe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gxoggqywk.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqksywrji.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gblydeveu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gseobhtsy.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gayauxfza.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkwktjxho.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gspwcgkfx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gyqnblopp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/grqutzfcc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/genjwjzbr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gbutqsafk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gmvweysxe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gltdvpiga.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/grwibmgzw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtxgntvvs.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gsrgnvsje.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gwtmzizzb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gditkciym.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gaeyrrzpq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ghurcwdvn.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gomfivojf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gkawlsxls.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gkbsxlptp.sHtML


<!-- 参考信息 -->