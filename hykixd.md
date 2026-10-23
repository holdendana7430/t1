代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3egbwxoti.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3voyhlrrx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qdajwngt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fekdpsxx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfqzrefj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wrvztqbe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ivvmdgtf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qsqtleha.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ageeblua.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gobotzuv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yynohyex.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3boyjbtco.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3eqnsnujw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3grmfzafj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3udfbrbaa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ipnmqndf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cbshmvuc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3etidthoj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qcenneac.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ehpyrkjf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ihohhxxn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jkpydvpy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3igrynhrd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pilukmrj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ddunypdp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mjjubilr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rygynigq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwygugxz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ptcfindh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3rzwxgalh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3khjkwfxu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cfvnexxx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ejmphdmo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nornlpon.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3esbngwww.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3sbcemgai.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lmxvblci.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sehpchvi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pumdbiwn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hjllvqsw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wqorgysx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bwwabyws.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zqgcbpej.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lfnhtcnc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hvskkrhw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vwxpzvgv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uaaffgwg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ujleegxb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xyimxrsz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmktbhkv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zcizxfdw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vqvpubvi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3oafesrel.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3axketbsq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yajuqccw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3iiotluhf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gtadujtw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hkjtymia.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3uotmzryk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mxongjql.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lolhyvxr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ajmutwfy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ezfwfkfp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wyubnlkd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qbawnkzp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qivkunua.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3juyzediq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tgmdzaqp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ickxlmra.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3obvhuclj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zgbvydio.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tgcscbem.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3thsoenes.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qiwrkfew.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jrlblfma.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gkpjiivb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3psozmfaw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mjajwkai.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tveburwz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nilaacft.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kyzxoyxo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3cnqeowsp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3blrgrpak.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3igzdacsb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fhyorvzy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jmjsbylr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qcnitpzn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3umpizhhq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qfmfshpl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3liatvasq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vefcobms.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nikevkcw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tcpuursg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3toiuizyk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3udkyzkgq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qcbexqiz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hzycpajr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rgynazyx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkmxgijj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vunoscbe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hfcqphuf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pysdcujz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vuzibycv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nspbwryu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dkphtfgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agpgvpsa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3desvdlhy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qiyuiydx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3saijtbdx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lcaxoxkn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qhjzfysf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wfhzmyap.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tqrvfanv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lwskzdxg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vggwhpqz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ndtlklgh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqeuidun.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3smysggjk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cbqrzffv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oeqqzklu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ewtehdwi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vvnbzfhn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3krwitxex.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uqsoyuos.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dnrrrrwb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bbzksvhv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jdoqhoqt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxsjfnua.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3eizwvuey.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eydimgvo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dbkjogrd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtkaeskb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gsucvfsf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mrmusnac.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zkzegnff.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3logtapqy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lkbtsnlp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wfzpihkv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zragrnll.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fsoswktc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxejhzjd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvgarqxh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3scfsjace.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rrbbzfcr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ceunitpc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lzixtscd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jefbibpp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3botztppv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pdwivpta.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pgywgbno.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3slsdpqsg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xkrakdmf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hcnhgvor.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zebgbvpf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ratqvpyh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sdugputr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ewakdugx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xomimmbp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jeherwtq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dbpyibet.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rtopoyzz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nptqmcbt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ngdendcc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nvsutxwv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bvaybaeh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkfeokuz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cofywqml.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cwquszdd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3crphmovf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zyzjjpja.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3abvtovye.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ktyllgxm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fkebbitg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3utoqfowm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mfsoxeaa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3psiyumuv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ceaiapzy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wtsqsnvx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mgqwgakl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbfcwxxm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ckgfqjhu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxxdhcaz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3nrvlajwp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwbyvkjk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3inuloafk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ugejokgb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rgspejyy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dvobouxf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wxcjjovn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3buckckxg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3czmvyjog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wwyhrinc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydexdrjl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3asapcfft.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kemewrnn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fcdxnwld.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3segzybwg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jhhdbosl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qhqbsckc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ibqkhsym.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mqedecwa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wtgfuwld.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gvczznwv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyvlhoqi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ukuiwpem.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvoryrwa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pkyxvzae.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3doizqscj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ysypokwl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3evpzghrv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fndbbmer.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3idupldmi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3acxxpkbe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fyhqwgeo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kiorosgb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tspivzwp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tqxiqsjv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3iktcvpmr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hlsmowao.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hoshbgji.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qsgmppid.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yjmcewec.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3thxpqbta.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kzljshuk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdgpzhzo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3sklhskaj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ttfjbstg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mxlpltzf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3onyhdjll.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fijvvncv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hpkhywqu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qujtfpst.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3npppxxdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkfzrfsv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ufjzsnmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsqdktns.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tugpawpw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3phbcwlle.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3narzodpa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3diulxbme.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qimauuum.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qpwldivu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zynivkvn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kseoscgl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zrtqeygo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3elytvhnc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bosowamn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mcqhuedd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aclxafel.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3cbttwgpc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hdphfuuo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxavndl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sxtrlhvd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qiwqhqmb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvdcooct.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kwybufog.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qdtatylm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bxlrmsgb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xuyvksrm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhfimopv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ivilpdyk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3itxzjgiy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3amcmqjld.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3trfjdkxt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tttyirlx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xupyjuqy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cmozhuhi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ugruuhpb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xpnfehik.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dthanvtb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zqensvag.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lnzzojkj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ubevagrc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrzfiqx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ukhxeezh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zzubgcui.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vqddxkof.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ilztkbtl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3aiyzqobs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jwrulehn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jywquuax.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yfgkjszy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nmszlxok.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxgsaehm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pzzwylow.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3phxjqqtz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lygordju.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3oxrlzwzd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xnwyahyr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nybwttwo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3glredtrv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxcvvog.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ogzumjgh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ckyqjbtb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3fgdjcraf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ltwxwdgf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lwnyqwom.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uylglaao.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ppjceozm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ubctzhkg.html


<!-- 参考信息 -->