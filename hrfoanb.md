代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gldiuccdg.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeyxvjzc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqszhcxks.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwvfxscra.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gvjwckgrl.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gypnforiy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxodpasue.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gywigwcri.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gqaqtxost.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtigbquus.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzolxysxv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjkzpjbz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmntjwoi.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfybzbab.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtrxctloe.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpplozda.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjceoobn.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gogtrekpr.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gsotabsvj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypnurlsc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkneclkfb.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gieulipgj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gjzeugudj.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfwfagvf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsayavve.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gynaleouj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtzlbwe.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggedbtwtw.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/glewjwbmi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grtwcpjgo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrtgbnao.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gtklaalqc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gruatpucj.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gpwqhorzy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/glguuuyut.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gpecqqrza.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdiajpni.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyxnxuil.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyfiljbj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gwmzdyesd.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gkugddueo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdemyzqqk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkrhmtth.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gsliecqgy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdgqmgxg.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/glmlvrzsp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkezpyqt.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/grrewqcpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtklvqfcq.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gfhwzrlpl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxdkulrp.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndctarii.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gasynizmr.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/glewhkrfi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gosyjlhbo.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpunflhw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gwsqfsgkp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlgprsgd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gkqmasazy.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gemzdlcqz.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gacpttbbu.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/glbbuybhn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdphptys.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsnhiloy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxglvtsep.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gdecbdreu.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqpzipbe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlxbgucp.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gucghrbkr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwzcdflw.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geuaqhiue.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuevocdj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghnjplbzw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gipmztmba.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gywozotvg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/godurpzrr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyizmggv.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/guecxkzki.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxayzzdla.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilqzwwni.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwstadhll.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpygdglwp.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ggxsvwtwo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvdvybxzp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gelvluumu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gtukfvzep.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchzyccbj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwtvhthq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gouehwlzh.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknbshpn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gtulddteb.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggonnthra.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gmnygqrko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gusmjdbhp.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gawvauvue.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcmcninv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gggyhywna.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucgxqcwa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxmhxfnc.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gednlnlif.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwinokyr.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgcpuco.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gecqoewir.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gjsmkxncl.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhfbmxdw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsyeonnq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdcadlkeo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvlstdwj.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gymjhuhka.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsisrmtt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkfegrzuz.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/guxjxiggj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzivtcooz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmlcfkut.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmalxbkt.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsbjbnnx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/ghkuxouyk.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gvgtzjqtt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqcspavb.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdoshqtrg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkimjcbk.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyebkoft.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxcrhdzt.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/glzatthyf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrfostjr.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpajnzim.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gihysfqun.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcvsnura.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gynjgiwgr.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcmsfqjtd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gayjfesim.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoupvzic.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrtzryws.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gamfmopkz.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjlrnsns.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gckbfnfkx.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsurmini.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrenzywe.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gsmgnfwrw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glulxddyd.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gfqwzvseo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gjjkuwlkw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gmydkwsdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gteifkmjh.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqyyunfe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkwhlwpl.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gchkxbkpx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimfszfrq.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrbxwook.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grggoektv.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwhxthys.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhdygucp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylieubep.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkasyqwfj.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuclowba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcehqkxs.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geuczlzwk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpkjlzlwx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxzuwscku.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gpaiprtvc.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gamoovurn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/geoqtickv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwzmoojm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzolvprrz.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiilsghm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/geigkjrmd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkjmwjiu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwafjaoh.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gujnprmto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxifhxwel.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grmitorjh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxrxnpqp.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzarujmg.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbhvikmj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/giewcphlp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyzjkdlz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/glygofqjj.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/galbtlehk.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvyngyyd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gksdfnebs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gylbgrlij.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvhskbnq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/guhtyomsy.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gryvwqqjn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdsyhvit.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gnjthngdb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glinpxolq.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gqytwxwlc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnvntgjh.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gddnfdlvz.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwddenysq.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gyidwoyta.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvultxoln.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeckukea.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gdpqwcnzr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsquyytc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxuswmmg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmnrwgkyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtypszyms.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteknqnkx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwahcsnat.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/goktmmdss.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyrexbvxc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gofwvjhco.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjtywmru.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ghkdrykhb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gilfkqjbs.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuldoedn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgssqbtl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqylnsxh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gotgixvuj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghazvjmup.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjqbpjre.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqjmdjvp.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/grjnacnww.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwjtuvrxf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqapfpvda.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffktmssg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gngdctecz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gvuwxvhvb.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzdovwax.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeszecty.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gbnwcixgj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geekuonni.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gavnernem.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxsgoezfw.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gykjrbdtg.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/glhreoela.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnobcupuf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/grbxobgsp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabunmzpv.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gshykosdy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkpptvis.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyiriryue.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxklmdc.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gqqxndiwj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gutyjujeh.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gludxixen.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gusgyeoqy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gcidnybdv.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsrtwjpae.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gcegxbyxh.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gvihrchaj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxbvtphbe.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveppsmhe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuqsyqfy.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiyneshr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gdonshrld.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzmgfhd.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrcanezr.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gauuhmusi.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/guhrkrrhb.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkjgjtvt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxnuyfkfg.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpubnhwyu.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltmnqztb.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gycnfgven.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggloifrfo.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhdjwsrh.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gtcuhgcfr.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqavmjwva.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbmtuoav.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gohikuwaa.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfaugepz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gysubmtei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngjreecp.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/ggkbsydgp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/geirirkzp.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnoeczxm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmamtslrj.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggqrsfqed.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhfwwore.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtocfoacv.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhyvdnlk.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grvoqnjan.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/grkjkjnvg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwwdprug.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gvujetvby.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhhntyzl.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/ghvyinkwt.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnmfdhay.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/grpbpadtu.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkdtvcjok.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdojpsjt.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/goapiiirl.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gltsfnwxd.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbfflgcco.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/giezofbdf.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlxwyhfx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwexxjkzr.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuzuzafr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagmhfiqr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzpiknnp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyicrfsce.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfgcimlsc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgqhffm.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfpgtfzv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvdpehnz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdxopvuo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrhnkgyz.sHtML


<!-- 参考信息 -->