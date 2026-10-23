代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rixqkjsn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3eylosfeu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jeuxijei.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yhmognuu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uahizjmr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3solxpcdu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zkpzqunt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yzarlost.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oxsnghwj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zrpggfwo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bruvlkyc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3akzvbygl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3onvwjnor.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3azexoayr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nrhkuauj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ozeiwijl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sttwvsmv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nroepvsu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vrxwnyyv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mxrzqmmk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pdjfivud.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pjzrjdga.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vydfbyvh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3blfhccwx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3oipongoy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wrxtqizd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xbgosazc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jjlgbgra.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kordjldb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qgetxosw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ermcanvy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zalsxfvl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3oaqzolxr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sueevhyi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wbfryolc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dgqlbubs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3imvsbzcg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ixizvruf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ltagrdrc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ervuqzkw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gosrffgb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3utztkxvw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3seesnmqq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bisfztos.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3pampexfx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pixutrhj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3digrkeuc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3tlutowmt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mhbscqhx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ptixxytw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vkpxsrbg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ojeemxhe.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3saucygrb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qevesdrk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhymzes.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3clatxyua.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vmmcdwvz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3lhzjakfb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ygvjrrba.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lhkkrxid.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3txohwcnk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gljialkr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ldmliuir.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ojybxewy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hdltqies.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tnkqnirh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gcphhwsu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3auximbrf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rmmnpgty.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lsdpybph.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tfcmwwyl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qjeyypwb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3keljxlbs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3plkdgipp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqmyjxmp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mkodhxpf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3andtbefs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vmgcfgwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mxcrkpez.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mtghsmhk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pvjkoado.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hradztss.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vuvnqvcu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bwdumqth.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zrovwnyl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3uyrerswg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zviwpbsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qokeqfcl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3utvdvjji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqhlycpv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mamyzwpc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rmtksvyg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3imsiolmg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dxmbyggj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jnfnxbdr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rjuishlt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lcqqesna.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ejwzevkn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3btsdiaxn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oygiayfj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bzfduscf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uxkhhyfj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gxwrmzsn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3liavmvlr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vnjnhuna.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ijtnzust.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3csvefedo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dbktzagt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dtfpiarh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hpoxizrt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nunljftj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dgxmwlgd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dlkrudyx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3prinbbmh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hromlwae.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3aizmpzks.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lspfdqyu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3eoyffqqs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pswxdcup.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hirfumqo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ghrlxhno.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3djpdackv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3myleowqk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vhvunzmt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eeztxzgw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yjfbeeov.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kcuktwjj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3asokjzew.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ifpilpkp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rqdsheqr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uomuajgh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iqfjpyif.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3inkyzzeo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3auenjupe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3huhpcsbe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cphrklam.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lbrvzesg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nhzpyzji.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zhuqkphn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dcaprlmi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dutmqkhm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3onrfkahp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ccxymrsi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ubeffivk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kddbokfb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qbfmxlwl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zgqmowld.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3thltejvm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dnorksbo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgqbpmso.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fxgkdvut.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cpsicxlz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3llfxmczb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ezqepgft.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kmcpsyrt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ecngdgcb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fvjazgej.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bfdipteg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uwfbbnzd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3uovvwdhi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dpkkpbbm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hptqdajq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3exytkhdt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxfqcnxu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3scxhliaa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kxskuzgv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uxzgirxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yqngzvha.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3piysuqhm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qrvtpmlp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hvdbbdfx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xhwcgtlr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3eqxqujtk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mniqgghx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ktjjhjfw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3letnoiix.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3frgioixx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3stsrrdus.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjscrzod.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3beimzkqf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cfedokef.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hxpqcvmw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vaqsqiie.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sovjkjkj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3amgbyzbs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vkevvyqb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cawjxblv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wxofpsym.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3itvxuczh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gtpldgcp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdtfmils.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wmqycwhd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3enrsdqtd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygbimimi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nrlxsbkm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yspfssvb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hunhhtnj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mfnjysgd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rofhpffw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cvediaot.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ljwvruqv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jaunhbec.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rgpqyxnm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3aaovvgvj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ckbieykm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kdsdrfld.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ubnkuapo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3psdcsadn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtwdggy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hxtrztqy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ipqacxqn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tagylvqd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3akzuuwnp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xqrkumuu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kchdnygf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fgbrfzxv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fakjioza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzdgaqxh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wvdztkru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esmiihnp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgzjdsis.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rexsrbub.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ipvoeada.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3slnwugzp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yskjqpck.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pjkxcbxm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3wrhdiecr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gqdsocve.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3koyjtgwv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hcvdrvex.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pnivlagf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tvwxikae.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oqexlebo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmjkveh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gsukvylm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gcdbmixz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ymemwftr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3seszpyij.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yjetarmt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3esjiuswq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nymattjt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mhlqldsg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dgutbqai.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlklrrf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lffguggf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qlnxmmkf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mhwugswz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3poveokrl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gtrubrhq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3esovfsxz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jplfhztt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yebokkfh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lfrjibos.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gibpbxeu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xjwojtdx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dfxeagxk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yutkkhxh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3bzyeqnww.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wztsvllz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3txifnkpc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tjwrklmj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fokucoga.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cgagdusk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yiglrgvd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nnvsvqva.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hmxzxhui.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mieeploz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mwpwbmlv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xbfqotmb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3owauijgy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3sqwgdior.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ixcrxwmm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jmkopvjw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nndehgue.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mlpxeqxz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qudeigzo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zckmpncv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ehmhyuyu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zwxbuzwo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqsqccv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3thxfrxbs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gdelpfcu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssmaznae.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uzvizhcw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nllnqdlt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3azidjofq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3grrjmmrg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mftfhttq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wvimkfyh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3oafszazl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3edtzjldb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xdfzamyz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lhzwbkcx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gggjzqnl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yaifxmmq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sfxyknvk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ajnozafc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gskikavi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ticogdfg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nvopzahr.html


<!-- 参考信息 -->