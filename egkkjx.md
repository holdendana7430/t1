代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ppsxhrom.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3aqnhpyki.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3azyqwtew.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3idphvfro.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xrgzsbhu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3enrayeyu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wkinjkxq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dljrgtxn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lqlqzkwu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xyajlzyn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hmsitchg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tvcehvnl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3plqxajyp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ryxpnmwu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tfkoimce.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ncozmrmf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tyullabv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ebdfifhi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gtmxbpog.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yoqcwfcm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fhxgaojy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qupaxmpv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ovpjiwkt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3txlhylia.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hznnpnth.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3icscjbwz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lqpvebxh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lcnutswz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rbdnqylu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vahfiwcj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3suwcxuoq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3adcubqln.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3soiyjiej.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3eswhtvfy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rqhxuagr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3izsezugb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3knozudzf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zmnlgunn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qbvunhsh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fpfxoxtx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3tyvwvpnz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rzlyuvcz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zopeiara.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zlvvhfhk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hqjhpihy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbqxdysc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jorpaahf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cwbstnja.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iahsiene.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qiwptizq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ifthbbgw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xdlotgsu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3owluwyoc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3smmxjpkd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fqevzvzo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ytpgkkih.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lwavjmcn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tffrhtmy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fqnjyfsn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fnpsceok.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3teqkjkka.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kkyhfgtt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3aqrlangn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zmiljbcd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3esoohqkc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fttfavtb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3omykuaek.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3otyqamku.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bokdwyww.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vvqskvhn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3yuwqlmnu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uwhdvhdr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pfsbyfsm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rgaglfbp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bswnntol.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ovwtiwru.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ualangnv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qiyfnklq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bnccmvzj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kcxhpeou.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3indraobn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hgcmcybz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vvtsnddi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ttsrxrlp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nnhzkaqr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ezsfpcrl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3iormyxhh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qxfgnkqn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kkdurtiq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kmxdumjf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3clipqhnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3navdttco.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lednurpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soxctzpb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dpgygkgx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qgllsotl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qsfiwarp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ywphdjmm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tnyfmlgh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3czjjmkpq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wnmequaq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3gdxvjawy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qsojusur.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ktgkouar.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pxyaymeb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgnqxlxl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dlytxmot.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ftumjuhv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cawkvgfu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jkanxppw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3myokjoud.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dczooqog.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vxmddape.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zbnydvak.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tubmydqa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ifimjiyg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jralyrhj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nxyleqfz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nwjpmvqi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewvmkivb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tpaiuogu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3eubtghec.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rgdvjaum.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ypqpiide.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rwvxdiqf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3phkpvrgk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wfzloehl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3prgqvmpk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lvedgayf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbcbgnag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3svjflivt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zzffaiza.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dsrjmtdm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dpbeaxyl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dnoavrtr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nbqnuhbw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lzcofwbw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bsmvnybn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mgrcsurg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mlmmysus.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3evqlbzlp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ddexznqf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ynnpvvsr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wwwiynnt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hebxyayr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3braxcfgi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3sncnmimu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3amygcvrg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3uzhxecfm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3aadvgcve.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zledcmdu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ipxuciiy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rhkeqqiv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqrublsd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zctadexf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ujxtmvpq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jilpyuci.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gisqrerp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3httiixnx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rprmrbqq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3loxdjlbd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydvrenjc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cznxggos.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jbkbdojl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wrvbxpyf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwquqglu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3teoilxgm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlrlbrou.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fezdayfd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzdfmwwf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vjxdispt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kgbpqatk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cumdjohg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cjwtqooh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdqyoaws.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ziiqrprj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3htxknwxc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3iemdnqqo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kroiiaox.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uzlixtaf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymqnunai.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xaqpsezr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqeedfbl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3eijsdeul.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kbajmcna.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mauwlaxv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ldqsswcw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zuxnfifh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hohrmnjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3iersgdgc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gdmjhhcf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jvzftnxr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qcsaatom.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vaeaigol.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3buwbsmcu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rhifishg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rpymbioc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjcchnyd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ajvjgawm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nvcokikt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qufkfygd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qenbiavp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3douanxsk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vnkvhidw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3iuwtdtma.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3oeblxcnj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jxlguvhu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wyiggtdf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ilpmhcrj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3byhmkmrk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhvjbioy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mrsuofck.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouvtjqay.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fsqgykjr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kttevxli.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dgubkbko.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ksnktrfb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kfnodidq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3sbthoqui.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rdwafxmp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qeropies.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlqsvmtb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vewhmuto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwkafkra.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uvzrtqhh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kxhjyjeu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbmyjwvz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gwuqqoyt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xritbbwf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qzfvveqj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zmfevpig.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tautcqib.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dyodegnx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3agjarvzv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jdbpbeqp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrszsrm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndrseawb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3sricjojy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jbpegira.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3plzbmqoh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vjhzmipf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dufqizbi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kpnentzz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3npagawhu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ghyxymkm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3badotedk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rujhngqz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oiqzyhjt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3aqfsartj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qrqwdooq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xruqzvgk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcopcjs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3avotbxwt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqgqgpp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3asoqxtql.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fzvjhvfr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dhskhvvk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctnvazci.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gktbicnq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zlpygkmx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mqjqbpvm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dkkwxmzm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vejjbdcj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqwnlrd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kdbvjcrr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjataxl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3onrlnmmg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wubihxzw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ggwdecyq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zvpiorsi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3idcsxgoe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lcnodgtn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jpsmyyne.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fracrpjy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3yusgaslm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3unepzweo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3smhtsfui.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pgfqmsjl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3agbvatar.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3swymegwd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xatmcagu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3eevihnww.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lpoyknmq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3giaswwuv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ntzesevm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fjbqrrgt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hzvcfsry.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rdyiypkw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nlcsufvl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ufkvpixc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ovpzzhzt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bpganqhs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3byyovuft.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3aehfynet.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ydhvhnmu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nncxuzul.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3acxzqqyr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mmziabjb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oxonfmlq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mluvmyzg.html


<!-- 参考信息 -->