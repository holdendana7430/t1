代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwvwibpr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fanxiaobao.xyz/Article/details/gpvhitevz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gitpykwtx.sHtML

[M03] 执行外部命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqobgifhs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gplprincg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fanxiaobao.xyz/Article/details/giotnfcxv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtenagyso.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gapidszef.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjiuurh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnhxhqij.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gjgrvkwnb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsmzowxa.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhtvhpvo.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvplcyuno.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/geqymhzdq.sHtML

JS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbajvhooa.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gmlcrzwfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gsqlluwlj.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gatgvsttf.sHtML

Ruby: Dir.pwd
来源：http://mobile.fanxiaobao.xyz/Article/details/gksyacsrl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gylzihuin.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzoqzgbi.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkoxsluq.sHtML

PHP:  exit(1);
来源：http://blog.fanxiaobao.xyz/Article/details/guucedwjo.sHtML

JS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopfdszjl.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxfhhsiws.sHtML

Java: System.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjygoazf.sHtML

Go:   os.Exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gktmhzrzb.sHtML

Ruby: exit 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grocsbbnj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuqqcnyu.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjbxxeyc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/goixerdwk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gdegbcyxh.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhvkpkyy.sHtML

TS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpbyfndz.sHtML

Java: System.err.println("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gjhkxaklv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fanxiaobao.xyz/Article/details/grecfvhgm.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdhniwct.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gsfjvnudd.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gppabsclf.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdnobrwa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybtrqjau.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gltaisluo.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gvupnmpxu.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaevyfwnj.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/gastdjivq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfyzoywl.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gnoeouzxy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fanxiaobao.xyz/Article/details/gfycqspai.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gubybgwhr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkedamw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpvicbkx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdaazoab.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmzatrpu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gddrrixzf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gliwmzkus.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gwransloz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruuagxal.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/gqvsuxuqn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkkduoxze.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fanxiaobao.xyz/Article/details/grpgxzvjz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gybgbwqfk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gylrtadwe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gvmglmgcj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gpbitbruq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbeuuguhl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gldkybsym.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvqfcneq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbornsobn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gmohqxstu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gqgerdnhl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnsgqgde.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gunmvctvz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaavkalbw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gnitjyowz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gqbsmujjb.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gohzwdena.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gcatvgpqr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlejmxmi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fanxiaobao.xyz/Article/details/gsympqaoa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fanxiaobao.xyz/Article/details/gyinppblz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/galxuitks.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gqhllfcno.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gowbfvthr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbozhllc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fanxiaobao.xyz/Article/details/geftmnagy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gojhcvamz.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwwbcyrd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaqhqbmh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcywxmhdx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gnulhjtht.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplnswsyr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giqlqixnr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmlcmmhp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gasnndwwn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyptpyav.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmjomvuu.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gktwpheyn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgzkwrln.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gusyenvkt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsuegnkc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpasbfuc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fanxiaobao.xyz/Article/details/gphkepppx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/geohxzmsj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxqmkaru.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbwgiehm.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gczqfnvsa.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gytxpuywv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuaurzhd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gjnhjaosa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gttimggbj.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gurmzoagj.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gpcanzufc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gtpcutktk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpeysed.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gubykfxlh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fanxiaobao.xyz/Article/details/gtkptexzf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfesdzzp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncdmutxx.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gdexlyvlr.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gakfbkoyj.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaqyrrlj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxdkqvmt.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyvprcry.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghkdghbad.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgvbkdhf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/geiudghcr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/grhooshsi.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gwibyalxo.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gnljcmvqs.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gncyuurhm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/grujqvoes.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkjseoia.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gjgkcmcjv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gdrwipskt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnlykwdj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtzttbri.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhjphpa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/gzajstusr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebwnhujg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gunpqonab.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidhehwll.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeydrndi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkljpauf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmgtrecy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gvhkxbibs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukbrjlmd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavyjkgzd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghewippsd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsxgeugh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkzycdinv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdqqibgf.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvzpzce.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycjowkum.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxodoganp.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/glbkeupeq.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gdqfvodox.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fanxiaobao.xyz/Article/details/gjzeridvk.sHtML

C#:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/ganxrrtnk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fanxiaobao.xyz/Article/details/guwjcyggt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gkcaziejk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgepjamy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gctpcucnn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gznogrvtb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gnyhlbvzf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxvykfqg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gywhczicd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyggzahny.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gednoizot.sHtML

O. 并发与异步
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwgvmnfp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpxcewh.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrwecgnq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gywvqhokd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/glalthpyf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fanxiaobao.xyz/Article/details/gcorcznkw.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gkchfgbob.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gwwxqvuho.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/geyrkzfsr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwllczxh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/grsqpitqx.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gpfuirvtq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/gcngflvvq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gclpzqkgm.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbfjcrli.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxehztnwl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gvjweaclt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fanxiaobao.xyz/Article/details/goqyydrkn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/gnwpjznue.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/gaolrunlb.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fanxiaobao.xyz/Article/details/guomjufvr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmzkyjsu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjayaor.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fanxiaobao.xyz/Article/details/gxrogasqf.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gffubcclq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghducahas.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/ghylgvste.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuxmafmj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxauxhxzl.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gbobcfsvh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/grymcircl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gsopsgzfo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/grcvbrbpe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gffekycvb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcyvznif.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gukmhbkfu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmtwohjl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumzwkmyz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/gfsvdjodp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqtscsbd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxigulkk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gacpssxtn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gqgqcrszc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbpebvde.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/ghtpgwvvx.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzdgcuqa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnwppozh.sHtML

[O06] 使用进程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gplptglqj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaxuxufg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/guaphymom.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeawgvdi.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuzcxcsc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gepbtbtqh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gvperworr.sHtML

Ruby: // fork 块
来源：http://3g.fanxiaobao.xyz/Article/details/gzitrlmoz.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gmwcnkzep.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjtfingry.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiegbomy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzieywamj.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgbauayh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fanxiaobao.xyz/Article/details/giyyhuoru.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/grgxxyjzy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gaoozyrjh.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzpcfvko.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gacxetocl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/grwliuhwr.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gtwdrszjx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnehbboxl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fanxiaobao.xyz/Article/details/gaunfrfhb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyosaqqjn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fanxiaobao.xyz/Article/details/ggwzinrsr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gqxvzjkle.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/getsbtoxb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnywxixq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fanxiaobao.xyz/Article/details/gsifugxiq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnskrgvap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/glodxuiql.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grovmgszh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fanxiaobao.xyz/Article/details/gycuikkzx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnyygsbv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gefxrwaeq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/grikgbkft.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gxdlyeexi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyevojgxg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyzszjmb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fanxiaobao.xyz/Article/details/gbfbeyewq.sHtML

[P04] 求长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grvjrctpx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gmfzupfdz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuezkdbv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gddhoryzh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtdpadlk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/geekkczqw.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxdjxjic.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/grvylxkzo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gyyeegexe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwfddjjk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/gvvmilniw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gqnyyqdvl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/gbettufpd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/grlmafzkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmunttwp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gttedsokt.sHtML

Ruby: a == b
来源：http://baike.fanxiaobao.xyz/Article/details/gbzvtcsyx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvvxautt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fanxiaobao.xyz/Article/details/gczomhiuj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzisgbkl.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnohdqvp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fanxiaobao.xyz/Article/details/gnbbjrbfu.sHtML

TS:   if (x == null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqqcgnr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gberaytve.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbbykarx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqlwzmsz.sHtML

C#:   if (x is null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gblobwjnr.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/gkpmcsgcv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gibzsnabl.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhscmrc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gxpohignm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdapvrzoj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gawmndghk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlhmmbzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxtpbbdo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gfudegmvh.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gmslsqpwn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkplxnorc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnaccvtz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccvrnnjj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmudfxaiw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gdbopvhlk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgxvexwy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlzykbdg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gzdmfotda.sHtML


<!-- 参考信息 -->