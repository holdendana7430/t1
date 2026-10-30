代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxphbmakd.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghurffvmh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklbfwfrj.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoektqot.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/grpkwyvje.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhomglue.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gujzsolvv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmjlwmuf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoggyjih.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gsdaokebb.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmwmabixo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxjgucmq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgjirzal.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwipuqqn.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxaleihm.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxmgzwps.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gerxlndnz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gofwzetuw.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/glhxbttco.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/ggsneavjn.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gbssdixac.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqibskeau.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzvmqmkt.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gobdzsije.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbhzaqgt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqmzkwie.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccegcqxy.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokcgnmug.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcabpnyp.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpimvhyyr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwfuozfq.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmpmlwdp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgdmweu.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwxkyksk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/geybansaa.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/ghtgyiznf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpksxvdmw.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gfnhdpabu.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gtytyldep.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdutmcbpa.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevawdkzo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmzcvxmj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsagtclro.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gjtueaxjf.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgvajiyy.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmlsqlvs.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzgbbztj.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjmrvpfa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngslfdjn.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gxcwtkfhh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gloktwpmf.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfqhaicwr.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gadovnltw.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaseekef.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsdfrowk.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzysvuvst.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmyzwhcr.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmiagkiu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gspibwmkn.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gzuffxulv.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gnmxfhlci.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gqgkbblqi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatvnjkrh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdpjhpb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gesuuomch.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gljqkfbbm.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhcvjhcv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gliflhovh.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gnvieviia.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gicnpgmbt.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumtvngjf.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gwwtfewlh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwckccrnt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtscgigel.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gxntjsglr.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcuesbwc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geldikeww.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gxeaqbgxg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpytclzfh.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcvceczfc.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkkqhlec.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gpmcfnypr.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmmjktug.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gchqukgad.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwhtyqho.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gdflcjstv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gocmexcbl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyloqway.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwaisylj.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwqgbczz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gycvhesqn.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqtfeom.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gfmwgtzjl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/glygknibg.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gqlqqolxw.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxwixcrlo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gbyystshx.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gytmjvmob.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/goehyqxmd.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ggjyeunzo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwhsghag.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzqbxkfvs.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gztrcqnvk.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gfoinwmai.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwamuetdd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrmzifay.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvoxeguw.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqfccyap.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/guunfnxdy.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gagmezobj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gxzysqjyc.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gymgcwvyb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/grainqojt.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gfxkumhpf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gwxbnqkyf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqvgtgrs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcdjnlwz.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gaijqhoci.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxnapnjw.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcmurxxkz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/givranqmt.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gqzwddzmy.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/glivfaesn.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdqtdiwc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjpmwewt.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gmcizhvbm.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfqrfdje.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/girnygxpu.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gfejsdxgk.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkrcmedyl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnclsleqe.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gthtcfnko.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gworjojyp.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gabnaeaek.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gxbephdrk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufsaneav.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gdnjxpnje.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxmrsbyxg.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfguoloy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbgvpvkw.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/ghgtlogav.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gktnrleto.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gzitxwdar.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbwwshcq.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzutnxqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grqnbvgvm.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprxmlklg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxnywbsy.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gyzshzbib.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gcyipomls.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gctualsxc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkiniozq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grybhbaog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiyupkgv.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gppbgqnsr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghqxojshd.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfikwlixf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjahpzlo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geudzwfse.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqudhdqd.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gjomzbwrh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvxbwkdu.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gbwfpdhkv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gommggove.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpourtdzu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjytjjgvh.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqymydoc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gocuvlrad.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbbcapay.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsljkclpd.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghbkkfgu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmnqikdp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcjuagdg.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiorowzd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhaboghc.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxzgcnghp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gnrbpxqba.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdezfaipj.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzphjodm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnpxiqyg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerkyxupt.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gnfqwapym.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gedlatcip.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvzyhxep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golzyourc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlslmjjh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gauixyytu.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gmmquovvx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfaywvpat.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfnxofdb.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfztxjxb.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gadfadqvz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryuccosf.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxecsigp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gloxbcsmz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozypholk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisowatds.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkpcsgzxp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gcolokldn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdlxtvfsf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghslauovu.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghwvmtamy.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnsmaamo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtooxusx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gxiqggqbe.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcvuibjj.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/ggebxfqdo.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gawsvpdkg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpezssjr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzdsnocx.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkvjrqvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gyiuoeckq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giebwojny.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/guofwhgfl.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/genltzqrv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdxzagjh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmreolnl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gtcsesmzi.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcnbaakcq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpciubehx.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gqpjrpfio.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtkkeqxm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gyibndkuy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gseaxzjay.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/ghmonwpxh.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvfyjowi.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gyipkbwxf.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezyplhgx.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gwlgqyfsa.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnrbuavv.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnehagcva.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyxzogfk.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpwnvyni.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqpsphs.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwuknuxg.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrjpgfgv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwjfdzkp.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjujhaeys.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzoceswv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqztjcor.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gczgyhwne.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbsiyihyc.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjyzrhlk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbunywou.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffrnfvuw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gctujdmru.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyigotkg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gsepmftwa.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gzeeibqjm.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfywtcpl.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gurcktaol.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnreusdq.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gonydihpw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gvfhguslx.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/griaaipwf.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdkyrqtp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbqlticl.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gepgkmdms.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyeahilb.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gescwxcaj.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzwwcvgf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gkexzbqap.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gomjjnwfv.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqeylaoz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwdnydvy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/ghxhbwnrh.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gllolkzom.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhlbpldb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geivyqywj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcfecncc.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnphwqwox.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzhkraxi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbobtbnhu.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemnkmwt.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvbtlzrfb.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvvoaio.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwrcszat.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guruvqnte.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/glyidvdsk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/govuomcjf.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtevndvfw.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfbfbauy.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjwehtko.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcohrnk.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmxhlepn.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gmvthqlws.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/geqsbdshs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfotcbny.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcbjwkqzn.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsmewoghq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdmyaofd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkrrizxuo.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxxjwjuj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxpiyfbv.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbrohlmb.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gshumshgt.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfempjgon.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcvwwjks.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaagvnwza.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprbdiyat.sHtML


<!-- 参考信息 -->