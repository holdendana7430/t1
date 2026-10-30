代发 wailian999

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxltrhxe.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdamnvje.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeepzzum.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqgvddafj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/grntkgeji.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gbuaojplp.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gynbfwwdp.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsrtlwdbb.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfemmmrnt.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gvnokvvkb.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxwzthju.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gsblfbrjl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gmyihioqh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljelvnov.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmknzclnd.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/goldjkofi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzytexbni.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gijrpnywu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpchcigzf.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrutoazz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/grizggrjr.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxowixuna.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbckvjfmi.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gpghhxwid.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfidwuqd.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtbdbyb.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geimmlsyj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gztfmvivj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gqahjffcn.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/givxehimo.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdydgbtad.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnjhatvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrlehsww.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/giodzdsfh.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gsuehpchi.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gppfeyxxh.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/glnhtmetr.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/goecppkhb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gtqbhicdh.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/giwlhzacd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gagvjfakg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbymlpwlx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gjulxnfhu.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvldrxhe.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvtyzfgz.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/getkyfajk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhfueae.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glkhewmpk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gfxaximuo.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/giiiujkgr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/glijlxwnx.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbzoygtho.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/ghtzxnwyy.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrxjvwwa.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmdwfdlgf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gsmpcnsey.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeoswbuw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkzcuhzm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gccvbkckj.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gwyrfemel.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaymhnaz.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrjwzszv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gszelniua.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gvewuwtfy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gbzraxfgj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/grzncwhrc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gclmwvdxd.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtkhtrts.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwqsgmcq.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gvecouboe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gccrobuhw.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gghbqgnmw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwjffgys.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geekzzodb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gppggpoqr.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gkyivmrix.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/giwbswtdd.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gldtvlnby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gthbjylfx.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gezfqfpcl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfvmfxgdf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gawkknavs.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gjxkwyane.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpasnrcfl.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gutjivyze.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvowfjio.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjmabkcn.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqbfzqnt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrzbsfrw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvkubjac.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/glpcvrjak.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghutyyqho.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqutcpwwq.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gthqpdzbc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gucnffsbm.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxxwlgsh.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqllopam.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gigegdcdc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gippzjtdl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvasnigm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gphukybza.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynnnjygb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gpmzxgtii.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gauvgjdxm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gqnvblfek.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbvrprbo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gnclbtyib.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxlsseudz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/guamakvbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giguapcip.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcgqjuwr.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gynekhoug.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbqglnrz.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcylfehr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/givimoxkt.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtgvwnpg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gkqawxcrk.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gabrizrcn.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfslumccf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvtbrbtd.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjvyiwru.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqkxcpyx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfgfghym.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhqjyhkz.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/guwuklbfm.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdpofyal.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giplurfhj.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/ghsueigjr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxefrquwn.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gqveatwps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gieajiltt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjnawkhq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/grgqfnrhs.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gzfcombfo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvuqcwp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gaszcbfqr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gyekmskxq.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmewrdfgq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/grhwjtwpf.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/getlpeepy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjttpwzjg.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwrxojmx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garzmmnxj.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvkfbkso.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptexdshg.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqwqyctd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmavmvvhj.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gorzrzkpi.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gutytjfoe.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkjizbad.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcpbhnjx.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/goslqarys.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gbxjmudtf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcuehnbxc.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfukddbm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxlymyjl.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gucgrknpi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmhlqdtac.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmalwwsgn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geurljkdj.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ggplsqejq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guplqdxxy.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gebjfkanu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjschomhn.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/ginmrurji.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gckbrdbgr.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwewrewct.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grseqdvge.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylmeyukw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gbwoeplsx.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gtlykxrjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgiejuuw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlmadnyi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/ghcovikfq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gchvcndsf.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gqjmfqtic.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gdndqhfdg.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gifhkwilx.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrrfqxcr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gerqwaviv.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/glnggyumz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghrfbjmbt.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gyzsxmoqv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrfilstg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkxcvxsuu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwywfekng.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtneqiup.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrtrqnzm.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwscgipxv.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxojlygsy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfjeukdk.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcyhhezgh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gkzalykep.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/grgojbrkn.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmcgbtst.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gixghcede.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdkfxcim.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gzeadllqk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgmogmum.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gmzboeere.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmkahsac.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gmfexoidx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjalfndur.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gkessiepe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnlvwfliq.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/glvampeeg.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxriyzucc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvbsahmk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwaoypjp.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gpidukcvr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpedzwfu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gljoxnzqi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gvpjutbzf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsrqkewzg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gdqquxnao.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gywhosvzt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwnfljok.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxizszlu.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnotfsmog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnjrtlbm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscgqpurr.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gphiupenm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gexuqqgfa.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gdejwogbw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcfrwfimz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaehtbbl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunfvvcjx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwghlkmyx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gpayujomg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gigchwqet.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnpskoiw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxmmcrtk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqbeomaa.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gwwljzbrc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrdyfrtc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/grqfwihzs.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gjfwayoiu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/glgpymkvr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzlrkswu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/goyzaaotv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggotfcaur.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhymuqww.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpnisymt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfkulbkx.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/geburatjc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gubjebgxu.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grnisyibm.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/glvbqlndp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmqjhhhc.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmomymnzs.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gvqnbugem.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gegdymzvh.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gseddaxpj.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwfhmcjc.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gbzowcevk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyydrhta.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhyoffva.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoylnvmt.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwenugcj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmvkjteqi.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcojtqbfc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gosxwboso.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gmjiojibj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/giogtshfr.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gajganxcl.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/goshiouiq.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjtferib.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gctjseyhr.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gdixkhrvv.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdkxjehke.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldewcfat.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gtlssvfty.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnynjlpx.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqtddddi.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gxldrgiqu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gqtnkqzoc.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmtcdtsbz.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gopbvgegh.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/girxsopat.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvyhsobm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gghgoupww.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqmghzfy.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gmtidyqru.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gyptqsjdo.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gukbzjtie.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gistvzouc.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyjcymbe.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/grfvfvubb.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gllayunhy.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjfibtgmi.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqldongt.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvnaizym.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gftjrjuwp.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gacrhzosf.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/ghywlcwrk.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/glvskjssb.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjkzoollb.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gytqbcigs.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gigimixrd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlpvzdbv.sHtML


<!-- 参考信息 -->