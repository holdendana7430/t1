代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qyeazvpn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3uuwdtrkb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uhdsbtds.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qgaxckuz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bzsfmapq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qunqgpry.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ryeblgnp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pocgnyxt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yjehudah.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3klrxpkpc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mwmvfqhm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3thdmmumv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hxvyfqka.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xeqhzxmi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wxhilkny.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ghkidyky.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rgwkwngu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3evwhoiyw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3czvukecy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3luozgdzp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxqftlrd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mmnstduv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dsuehnza.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kfxlxfau.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kvjbujuk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gsdahieq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tawhzijg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gycslced.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3oiiudmry.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jkklpyrc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3foatlqwu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dhaidcje.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mmmpahqp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qdhplqhz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lhvdptfd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gcqqehdi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xiuqoizc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iamtsgru.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jjullgeu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pfngyami.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dgmsyzct.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ziwoauer.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3unexapbc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kvggllos.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wqxcvczb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qxnulbql.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qtwenhvl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qzxhxpai.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wkrpjzwn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rktfwcil.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ubojmrzb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ttcpoqrf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ipnazlkr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vryvvfte.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgywimd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cisizuvp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3baxicmdy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vwqjbdpw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nxnnpksi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kloedaeh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zvldbzxh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kcvmijmq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3omgdzznt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3oqtawxro.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yfenadld.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fbhqzoua.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jpyncakq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xlwxszqd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vpuwuiiw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gnioeksy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pohmqwim.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gyewgrry.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3admdhsvi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dktuyjel.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3rqwwlbbl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fiaddgcy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3crbcufdx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnprjekh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uvwgtclw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xwfbubgb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fybwcerm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pucqtmxr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kwartesx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fpkosobj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vrvamixi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3mxtsxkfm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ntmkxtay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjizrjpb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mllpkefj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xowquktq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rfkwxyxg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bwkyrbqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3okcnkdzh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sephjiql.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nhlfgixu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yosngcud.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nhfmkqxs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wxrobodr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mnbqnrjr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nmqllzlr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3afdcfjkl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3grkwvdgm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3umzbogql.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ywsssiqt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jmagkkkq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ktnieqiv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3diwzxflu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3plctjeqy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qamhqwfe.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3njtdhjtv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ofbahcgt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zlbeipkv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nalbebzk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhwfdqum.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3deuuytwe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bggujjlc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fuwotztp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dzqalibq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vtearrbm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ftazzmwc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xqoodbch.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zlykbzfn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yaahehxj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kwqaelrx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3iyzzbvby.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhujwbwp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3basgkart.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgjfspem.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3cqkgifgi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nucmqluw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3olejcpvt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tdtlkoha.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nmwzofgd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nwrkuzqy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xpwyughi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zvuwpszu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rrgovcyg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nuopzpws.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ajfzposg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cvxqkxto.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dmxkqzgf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kyctzhti.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gadkoeve.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vdeuemvx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3riuqnaeb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ktqujhmd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3skbsqyck.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mxkdxiid.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xwscuzpn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bhposewq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vapuhxpd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jlgjkhqp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lvhnijxi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3llyctrpk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zichugwj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zzvbbsxh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yyzdihqv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3iecgkayr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ofirgxpe.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ybovnzhk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3thzxlaci.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3shcxqeos.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wxuvsqjo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoairaqd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vatdnfke.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iohcdifq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uuvziblk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iivkrunx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fxedxmej.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xobattwp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rpebqwan.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3piymladn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xikwcgkz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gmmviikl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dpqhbqhy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rexgewwt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vuheqshw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3btznnqna.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3txdgtblh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ccvadmce.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3viadabpi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3omyobkzo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rkxwqsnr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fapanlvw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vwwdxyfr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3diktnprr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3farcjqmz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dknxxxye.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3akrgwgfs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pufnaneb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzoxyxcm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gvryjbvj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oxvgonjq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oiiojeoy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3swteqvdz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3dgewqptj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cjfzrdry.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tvnkdqhd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3etjsykqf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cswtghze.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yicfyenl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yzciycot.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hjljobko.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3klxongrh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3auhzevei.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kjqnscuj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3maznncot.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rmgvrzqi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3sebgiiem.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gxguwqko.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rbfotfni.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vxbjmvuc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lpsykksf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lefhpkdf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bpcwfgnz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ykwefyxi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yskwwtbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppfjpqve.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tsznfobq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcvmhyug.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wwhdcbmv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3omgphzre.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jakqwlnd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bpcgbere.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gwejjlru.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jqagqaaw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jrlepaxh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kyqojvgq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3btubgiav.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rbcfzabh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gjrvckkn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lpckwhlr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ldecgfbb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lfqlmhud.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fxdowajc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zrxbmhkt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3adorhwsx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xycnapkg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rkvxpvua.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3twhjfyzk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3buiixmdc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qustakyv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wxkddjpq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psyoaxxm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hpoisrzl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bmwvhcck.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3stuajpvn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ndlydvff.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mrwqvvyu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ylbguiwc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yxnpploj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qujejlab.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hxorxeqd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xbhtictm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jrdqqens.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qllumufq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cvnuamxu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lduaqicc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vsoxigdy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kscalhor.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3anulwiyc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wnwgsfvl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hzphkaxh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mphwvrwf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3konjxcea.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sxzotnhz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vittozvf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3guktghym.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gwbfibft.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vacjrkcb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xjplfavh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3syenhnjt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xrcjntql.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mmqxmfai.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aevowidm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3clgeqfen.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3khbjfcuh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vfdagodu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3sjlvmjpj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yxxyfndb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jsiptlzt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3srsiwxmu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xzwwmyri.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3oytsbgnb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jxpdcpao.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lwytgaku.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wftuvysb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3yyynxydm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lhjoctvn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3maxfysim.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bsegwajj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ojgozssp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lcldjwic.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jdihlnge.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ouovfcjf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ztnsowsi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3squqbsnt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hamnxjoe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jmrmgxeh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uhahkxxb.html


<!-- 参考信息 -->