代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dvzfoseg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2enehhizi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nkzffdqh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2penkgajl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sxwufbfa.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vjeoaxxl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2krgtkzsn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ahvmjtmv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2uikbsgfp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qaaleppo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rtytcual.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tkpugpwr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rcjqoewb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dslrhwxk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2epawpfqp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bmkrxtsc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sijcrafw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2cexhduoj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wszbnbru.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2owroowrd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bndtsvzk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ytllzmkl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kzuvenhk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sllidmtn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kkbiubgh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2twtifkjl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qmhqgfkn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dlbjzfja.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2whebbswb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qoooogyr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2oniusqsa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2obqregzq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2eykevruj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhkdzxtm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2brhcnuqf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vyexwwif.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tiqehfnn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jztaumet.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gqhhuvox.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ytpzgsky.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kfjkapew.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozubfdts.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lgdkreoj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dvsycgml.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2egfzyyew.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tmynktxi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhachlw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2aqrbpleq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mvmdlypx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xhlfsjuf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2aafvvfuh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qqbqblbo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xaciglna.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ipvuhfjs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kqklgvym.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2guoveyav.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rzwundat.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2acojmcwh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rrsjnvte.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fbpyzysg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mpekrjnl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qviymcnf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ndtyathf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eadqpqkq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zxyibeqq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wzoafrni.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2arbenspq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xhyaecct.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yvqjejmj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2stiodmso.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zulaexaf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uktmjwbm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lizgezek.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gmxmioen.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gxiihahl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rygdodba.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2brnnjwsr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ayhiefbm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ujdmdese.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrujinpt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qqlpgtoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iecihrzj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lwpljlvt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tzemimsn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lctgvszb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2aqlftwrs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cmzjquzk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gvhzmsno.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2tncncqlq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tilqqpgz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zzpubclj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bgomykth.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2aihxgxvy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aoqondqb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kvtksctc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nczmulse.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cejggnjl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vukgqfit.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yqrhqcwo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lmovjjec.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rbwrdrwr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mrkfgrey.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ptvavyoi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sbashkxz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2byjfohva.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fuymctrx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yallrlud.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdafcqtp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2akjvejpv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wnhlpkaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zdzckosf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cbmidgue.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gdmgukgy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hjlhwqqp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fonnusui.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jmosinji.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pxoqhvzn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hihkvcin.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ejoesmvl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sckiuhju.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ducpwmyn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fxkzwslq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jqqffkgv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2trmbhrxs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tkcetliw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zocsaxwo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ylmuemys.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tcummhsc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2skdmvsuk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qoqfyxbr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xobzzavw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dqkvwjkh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hfuuemht.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2flwlcjqp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2zpqcxmmh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xrzsrgil.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2oeohuwem.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qasouhfk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qlrbxkra.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vrbytcvk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pabcbuas.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2delvghji.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ycvrfeyy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fuojzbmm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wkgpqtvw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yougvgct.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ohxobfpp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dojgbpiw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kalitiai.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2baevbgaf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2abduhzff.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hopqnyrl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eghogdwc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lsxiqqwe.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2mvwkejuf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lrxoazpn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2duisgrbl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nzytuppz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cynpjcpk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ldcmbqid.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2utnfjegj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dcqiwcvl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2chelwjmh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bjytzkhi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vudnvnck.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mxfrfzod.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dyztiimq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2udlbrhgv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2anqokfut.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yqwybkzl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qzqiveby.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2pbqggjbe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2fhwluuqk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dtzolobl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2evvweibh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ycymklhh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rfgizsqq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jbykxoas.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uhargbor.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntpsloum.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qcdrywfg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tewmnawb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcwpmptp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dpelvxqj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rtxxtnsb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xmfqpttu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ybinzwed.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dquaorkw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zskmpqbu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nufcetux.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zsiuglqz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iigxxlmm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvveyzjb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eeotgmxy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mbxhzuvk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lxuylxkh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ewluimvr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gcigukhx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zenyvmsx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2phbzzknp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2myipvxkc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bccepkff.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2heuhmhuz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mbhmcdky.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fcxtvjsu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hqcibexm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vcsgqbmf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dtqnkdpl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ezreypbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flrjnymm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bevocmwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euoykzjs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gzrteydy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tfpraiof.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bydkfbrg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qdplgefx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wvssnlok.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2oevpbhmj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zgolxwvh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xklsfqxl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vvhmsjqb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vlifexga.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ipefzlue.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dpqdcbeb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vpqetwrl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hhajqeov.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2owxuxxna.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uyyluaon.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hpxmurms.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uufanmby.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gxzflwsj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ljoeymqc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uciqyrcb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dstlvazj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fzknfdhb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jsuekuce.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ewtqjnof.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dspragfm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zwutahpq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qqktdpkf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2syzymfek.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tphgnwhl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jlwernqd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jgnirtzp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vtiqbrnb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yukttuhd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dlyowtva.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pzwersjm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2htwxsowf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kodvlbqf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2upvanzja.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oouoijrp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukqcnofi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zldyzuhf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2iqbninjv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kzywsxuf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2acebgmem.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rehjryhz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vtkapzhc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2opgxxipt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2itrjlprp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cbajxyvh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yxyxmxgu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2aalprxow.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2axjvuczm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ndhscwae.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nshdctxo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2aydscphl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2sdwwwdql.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nwqzjgcg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2whkiqqjv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ufwuwkqh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hzzmwidt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hrzyxnar.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jrkcbxbd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zobsmmng.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2oslsjosj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ocaimsmh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vnsqjwut.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wdjclgsg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gvxrsorj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ipaiimix.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbsbvcoa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xktewiky.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vjxtwqfd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tttmkzzs.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zwsmotte.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ciefxyse.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2svdrqoia.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wglmhklm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lxwywdcr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2srswhfdg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iavworcu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ehmgxxnc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pqewbanj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vgdqaevb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ztzjnxlw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2soecojxo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tdyziydi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2onuhulnm.html


<!-- 参考信息 -->